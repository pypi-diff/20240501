# Comparing `tmp/postnl_ecommerce_sdk-1.0.1.tar.gz` & `tmp/postnl_ecommerce_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postnl_ecommerce_sdk-1.0.1.tar", last modified: Tue Apr 30 13:22:50 2024, max compression
+gzip compressed data, was "postnl_ecommerce_sdk-1.0.2.tar", last modified: Wed May  1 14:28:03 2024, max compression
```

## Comparing `postnl_ecommerce_sdk-1.0.1.tar` & `postnl_ecommerce_sdk-1.0.2.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:22:50.801785 postnl_ecommerce_sdk-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1213 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6952 2024-04-30 13:22:50.801785 postnl_ecommerce_sdk-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6435 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:22:50.800785 postnl_ecommerce_sdk-1.0.1/postnl_ecommerce_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6952 2024-04-30 13:22:50.000000 postnl_ecommerce_sdk-1.0.1/postnl_ecommerce_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7025 2024-04-30 13:22:50.000000 postnl_ecommerce_sdk-1.0.1/postnl_ecommerce_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 13:22:50.000000 postnl_ecommerce_sdk-1.0.1/postnl_ecommerce_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-30 13:22:50.000000 postnl_ecommerce_sdk-1.0.1/postnl_ecommerce_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-30 13:22:50.000000 postnl_ecommerce_sdk-1.0.1/postnl_ecommerce_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:22:50.744797 postnl_ecommerce_sdk-1.0.1/postnlecommerce/
--rw-r--r--   0 root         (0) root         (0)      153 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/__init__.py
--rw-r--r--   0 root         (0) root         (0)      569 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     6068 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:22:50.748796 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/
--rw-r--r--   0 root         (0) root         (0)      342 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5194 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/barcode_controller.py
--rw-r--r--   0 root         (0) root         (0)     1731 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)     3352 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/checkout_controller.py
--rw-r--r--   0 root         (0) root         (0)     3381 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/confirming_controller.py
--rw-r--r--   0 root         (0) root         (0)    16940 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/deliverydate_controller.py
--rw-r--r--   0 root         (0) root         (0)     3886 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/labelling_controller.py
--rw-r--r--   0 root         (0) root         (0)    18238 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/locations_controller.py
--rw-r--r--   0 root         (0) root         (0)     4107 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/postalcode_check_controller.py
--rw-r--r--   0 root         (0) root         (0)     3915 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/shipment_controller.py
--rw-r--r--   0 root         (0) root         (0)    14089 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/shipping_status_controller.py
--rw-r--r--   0 root         (0) root         (0)     6428 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/timeframes_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:22:50.752796 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/
--rw-r--r--   0 root         (0) root         (0)      481 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      937 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/api_exception.py
--rw-r--r--   0 root         (0) root         (0)     1502 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/barcode_method_not_allowed_exception.py
--rw-r--r--   0 root         (0) root         (0)     1447 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/barcode_response_error_exception.py
--rw-r--r--   0 root         (0) root         (0)     1555 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/barcode_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1496 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/barcode_too_many_request_exception.py
--rw-r--r--   0 root         (0) root         (0)     1683 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/checkout_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1653 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/confirming_response_error_1_exception.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/deliverydate_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1565 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/labelling_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1686 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/locations_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1686 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/timeframe_response_invalid_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:22:50.754795 postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/
--rw-r--r--   0 root         (0) root         (0)      118 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/api_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:22:50.755795 postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/auth/
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1274 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/auth/custom_header_authentication.py
--rw-r--r--   0 root         (0) root         (0)      488 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      495 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1877 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1498 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:22:50.799785 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/
--rw-r--r--   0 root         (0) root         (0)     2632 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3612 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address.py
--rw-r--r--   0 root         (0) root         (0)     3503 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address_1.py
--rw-r--r--   0 root         (0) root         (0)     8750 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address_11.py
--rw-r--r--   0 root         (0) root         (0)     8667 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address_2.py
--rw-r--r--   0 root         (0) root         (0)     3871 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address_3.py
--rw-r--r--   0 root         (0) root         (0)     6698 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address_4.py
--rw-r--r--   0 root         (0) root         (0)      498 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     4585 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/amount.py
--rw-r--r--   0 root         (0) root         (0)     2153 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/amount_1.py
--rw-r--r--   0 root         (0) root         (0)     1614 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/barcode_response.py
--rw-r--r--   0 root         (0) root         (0)     4678 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/checkout_request.py
--rw-r--r--   0 root         (0) root         (0)     3139 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/checkout_response.py
--rw-r--r--   0 root         (0) root         (0)      567 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/code_enum.py
--rw-r--r--   0 root         (0) root         (0)     1834 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/complete_status.py
--rw-r--r--   0 root         (0) root         (0)     2366 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/confirming_request.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/confirming_response.py
--rw-r--r--   0 root         (0) root         (0)     3296 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/contact.py
--rw-r--r--   0 root         (0) root         (0)     3572 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/content.py
--rw-r--r--   0 root         (0) root         (0)     3507 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/content_1.py
--rw-r--r--   0 root         (0) root         (0)      438 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/countrycode_enum.py
--rw-r--r--   0 root         (0) root         (0)     3312 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/cpc_response.py
--rw-r--r--   0 root         (0) root         (0)      442 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/currency_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      576 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/currency_enum.py
--rw-r--r--   0 root         (0) root         (0)     1835 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/current_status.py
--rw-r--r--   0 root         (0) root         (0)     9549 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/custom.py
--rw-r--r--   0 root         (0) root         (0)     3986 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/customer.py
--rw-r--r--   0 root         (0) root         (0)     3940 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/customer_1.py
--rw-r--r--   0 root         (0) root         (0)     2421 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/customer_2.py
--rw-r--r--   0 root         (0) root         (0)     2772 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/cut_off_time.py
--rw-r--r--   0 root         (0) root         (0)      974 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/day_enum.py
--rw-r--r--   0 root         (0) root         (0)     2237 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/delivery_option.py
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/delivery_options.py
--rw-r--r--   0 root         (0) root         (0)      509 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/delivery_options_1_enum.py
--rw-r--r--   0 root         (0) root         (0)     1611 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/detail.py
--rw-r--r--   0 root         (0) root         (0)     3549 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/dimension.py
--rw-r--r--   0 root         (0) root         (0)     2912 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/dimension_1.py
--rw-r--r--   0 root         (0) root         (0)     1986 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/error.py
--rw-r--r--   0 root         (0) root         (0)     2086 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/error_1.py
--rw-r--r--   0 root         (0) root         (0)     1927 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/error_2.py
--rw-r--r--   0 root         (0) root         (0)     2247 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/error_3.py
--rw-r--r--   0 root         (0) root         (0)     2237 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/error_4.py
--rw-r--r--   0 root         (0) root         (0)     4040 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/event.py
--rw-r--r--   0 root         (0) root         (0)     1936 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/expectation.py
--rw-r--r--   0 root         (0) root         (0)     1876 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/extra_field.py
--rw-r--r--   0 root         (0) root         (0)     2051 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/fault.py
--rw-r--r--   0 root         (0) root         (0)     1849 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/friday.py
--rw-r--r--   0 root         (0) root         (0)     1578 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/friday_1.py
--rw-r--r--   0 root         (0) root         (0)     1952 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/get_locations_result.py
--rw-r--r--   0 root         (0) root         (0)     1838 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/get_locations_result_1.py
--rw-r--r--   0 root         (0) root         (0)     3078 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/group.py
--rw-r--r--   0 root         (0) root         (0)     6355 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/hazardous_material.py
--rw-r--r--   0 root         (0) root         (0)     2432 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/label.py
--rw-r--r--   0 root         (0) root         (0)     2501 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/label_1.py
--rw-r--r--   0 root         (0) root         (0)     3412 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/labelling_request.py
--rw-r--r--   0 root         (0) root         (0)     2793 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/labelling_response.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/labelling_response_1.py
--rw-r--r--   0 root         (0) root         (0)      602 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/language_enum.py
--rw-r--r--   0 root         (0) root         (0)     4602 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/location.py
--rw-r--r--   0 root         (0) root         (0)     6617 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/location_1.py
--rw-r--r--   0 root         (0) root         (0)     1917 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/location_response.py
--rw-r--r--   0 root         (0) root         (0)     1915 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/locations_response.py
--rw-r--r--   0 root         (0) root         (0)     2130 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/merged_label.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/message.py
--rw-r--r--   0 root         (0) root         (0)     2335 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/message_1.py
--rw-r--r--   0 root         (0) root         (0)     1849 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/monday.py
--rw-r--r--   0 root         (0) root         (0)     1578 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/monday_1.py
--rw-r--r--   0 root         (0) root         (0)     3301 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/old_status.py
--rw-r--r--   0 root         (0) root         (0)     4332 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/opening_hours.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/option_1_enum.py
--rw-r--r--   0 root         (0) root         (0)     1097 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/option_2_enum.py
--rw-r--r--   0 root         (0) root         (0)      811 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/option_3_enum.py
--rw-r--r--   0 root         (0) root         (0)     1005 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/option_enum.py
--rw-r--r--   0 root         (0) root         (0)     1735 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/options.py
--rw-r--r--   0 root         (0) root         (0)      887 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/options_2_enum.py
--rw-r--r--   0 root         (0) root         (0)     3155 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/pickup_option.py
--rw-r--r--   0 root         (0) root         (0)     2011 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/product_option.py
--rw-r--r--   0 root         (0) root         (0)     2177 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/product_option_1.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/product_options.py
--rw-r--r--   0 root         (0) root         (0)     3388 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/reason_no_timeframe.py
--rw-r--r--   0 root         (0) root         (0)     2035 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/reason_no_timeframes.py
--rw-r--r--   0 root         (0) root         (0)     2795 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/response_shipment.py
--rw-r--r--   0 root         (0) root         (0)     3281 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/response_shipment_1.py
--rw-r--r--   0 root         (0) root         (0)     3276 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/response_shipment_2.py
--rw-r--r--   0 root         (0) root         (0)     1855 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/saturday.py
--rw-r--r--   0 root         (0) root         (0)     1584 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/saturday_1.py
--rw-r--r--   0 root         (0) root         (0)    18276 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment.py
--rw-r--r--   0 root         (0) root         (0)    18866 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment_1.py
--rw-r--r--   0 root         (0) root         (0)     7281 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment_11.py
--rw-r--r--   0 root         (0) root         (0)     9494 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment_2.py
--rw-r--r--   0 root         (0) root         (0)      946 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     3025 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment_v_22_calculate_date_delivery_response.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment_v_22_calculate_date_shipping_response.py
--rw-r--r--   0 root         (0) root         (0)     3067 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shippingstatus_response.py
--rw-r--r--   0 root         (0) root         (0)     2231 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shippingstatus_response_signature.py
--rw-r--r--   0 root         (0) root         (0)     3451 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shippingstatus_response_updated_shipment.py
--rw-r--r--   0 root         (0) root         (0)     2547 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/signature.py
--rw-r--r--   0 root         (0) root         (0)     3380 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/status.py
--rw-r--r--   0 root         (0) root         (0)     3360 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/status_2.py
--rw-r--r--   0 root         (0) root         (0)      885 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/string_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      809 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/string_enum.py
--rw-r--r--   0 root         (0) root         (0)     1849 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/sunday.py
--rw-r--r--   0 root         (0) root         (0)     1578 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/sunday_1.py
--rw-r--r--   0 root         (0) root         (0)     2066 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/sustainability.py
--rw-r--r--   0 root         (0) root         (0)     1855 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/thursday.py
--rw-r--r--   0 root         (0) root         (0)     1584 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/thursday_1.py
--rw-r--r--   0 root         (0) root         (0)     3574 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/timeframe.py
--rw-r--r--   0 root         (0) root         (0)     2052 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/timeframe_1.py
--rw-r--r--   0 root         (0) root         (0)     2398 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/timeframe_response.py
--rw-r--r--   0 root         (0) root         (0)     3022 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/timeframe_timeframe.py
--rw-r--r--   0 root         (0) root         (0)     1826 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/timeframes.py
--rw-r--r--   0 root         (0) root         (0)     2008 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/timeframes_1.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/tuesday.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/tuesday_1.py
--rw-r--r--   0 root         (0) root         (0)      532 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/type_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      850 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/type_enum.py
--rw-r--r--   0 root         (0) root         (0)     2889 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/warning.py
--rw-r--r--   0 root         (0) root         (0)     2020 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/warning_1.py
--rw-r--r--   0 root         (0) root         (0)     1880 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/warning_11.py
--rw-r--r--   0 root         (0) root         (0)     1885 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/warning_2.py
--rw-r--r--   0 root         (0) root         (0)     1688 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/warnings.py
--rw-r--r--   0 root         (0) root         (0)     1858 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/wednesday.py
--rw-r--r--   0 root         (0) root         (0)     1587 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/wednesday_1.py
--rw-r--r--   0 root         (0) root         (0)     4185 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/postnlecommerce_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:22:50.800785 postnl_ecommerce_sdk-1.0.1/postnlecommerce/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      443 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/postnlecommerce/utilities/file_wrapper.py
--rw-r--r--   0 root         (0) root         (0)      732 2024-04-30 13:22:33.000000 postnl_ecommerce_sdk-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2024-04-30 13:22:50.801785 postnl_ecommerce_sdk-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.923831 postnl_ecommerce_sdk-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1213 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6994 2024-05-01 14:28:03.922831 postnl_ecommerce_sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6477 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.921831 postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6994 2024-05-01 14:28:03.000000 postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7025 2024-05-01 14:28:03.000000 postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 14:28:03.000000 postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2024-05-01 14:28:03.000000 postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-01 14:28:03.000000 postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.817830 postnl_ecommerce_sdk-1.0.2/postnlecommerce/
+-rw-r--r--   0 root         (0) root         (0)      153 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      569 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     6068 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.827830 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/
+-rw-r--r--   0 root         (0) root         (0)      342 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5194 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/barcode_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3352 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/checkout_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/confirming_controller.py
+-rw-r--r--   0 root         (0) root         (0)    16940 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/deliverydate_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3886 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/labelling_controller.py
+-rw-r--r--   0 root         (0) root         (0)    18238 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/locations_controller.py
+-rw-r--r--   0 root         (0) root         (0)     4107 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/postalcode_check_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/shipment_controller.py
+-rw-r--r--   0 root         (0) root         (0)    14089 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/shipping_status_controller.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/timeframes_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.835831 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/
+-rw-r--r--   0 root         (0) root         (0)      481 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      937 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_method_not_allowed_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_response_error_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_too_many_request_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/checkout_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/confirming_response_error_1_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/deliverydate_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/labelling_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/locations_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/timeframe_response_invalid_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.839830 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/
+-rw-r--r--   0 root         (0) root         (0)      118 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/api_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.840831 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/auth/custom_header_authentication.py
+-rw-r--r--   0 root         (0) root         (0)      488 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      495 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.919831 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/
+-rw-r--r--   0 root         (0) root         (0)     2632 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3612 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address.py
+-rw-r--r--   0 root         (0) root         (0)     3503 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_1.py
+-rw-r--r--   0 root         (0) root         (0)     8750 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_11.py
+-rw-r--r--   0 root         (0) root         (0)     8667 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_2.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_3.py
+-rw-r--r--   0 root         (0) root         (0)     6698 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_4.py
+-rw-r--r--   0 root         (0) root         (0)      498 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     4585 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/amount.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/amount_1.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/barcode_response.py
+-rw-r--r--   0 root         (0) root         (0)     4678 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/checkout_request.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/checkout_response.py
+-rw-r--r--   0 root         (0) root         (0)      567 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/code_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/complete_status.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/confirming_request.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/confirming_response.py
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/contact.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/content.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/content_1.py
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/countrycode_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/cpc_response.py
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/currency_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      576 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/currency_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/current_status.py
+-rw-r--r--   0 root         (0) root         (0)     9549 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/custom.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/customer.py
+-rw-r--r--   0 root         (0) root         (0)     3940 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/customer_1.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/customer_2.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/cut_off_time.py
+-rw-r--r--   0 root         (0) root         (0)      974 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/day_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/delivery_option.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/delivery_options.py
+-rw-r--r--   0 root         (0) root         (0)      509 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/delivery_options_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/detail.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/dimension.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/dimension_1.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_1.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_2.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_3.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_4.py
+-rw-r--r--   0 root         (0) root         (0)     4040 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/event.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/expectation.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/extra_field.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/fault.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/friday.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/friday_1.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/get_locations_result.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/get_locations_result_1.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/group.py
+-rw-r--r--   0 root         (0) root         (0)     6355 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/hazardous_material.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/label.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/label_1.py
+-rw-r--r--   0 root         (0) root         (0)     3412 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/labelling_request.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/labelling_response.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/labelling_response_1.py
+-rw-r--r--   0 root         (0) root         (0)      602 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/language_enum.py
+-rw-r--r--   0 root         (0) root         (0)     4602 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/location.py
+-rw-r--r--   0 root         (0) root         (0)     6617 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/location_1.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/location_response.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/locations_response.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/merged_label.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/message.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/message_1.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/monday.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/monday_1.py
+-rw-r--r--   0 root         (0) root         (0)     3301 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/old_status.py
+-rw-r--r--   0 root         (0) root         (0)     4332 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/opening_hours.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_2_enum.py
+-rw-r--r--   0 root         (0) root         (0)      811 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_3_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/options.py
+-rw-r--r--   0 root         (0) root         (0)      887 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/options_2_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/pickup_option.py
+-rw-r--r--   0 root         (0) root         (0)     2011 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/product_option.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/product_option_1.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/product_options.py
+-rw-r--r--   0 root         (0) root         (0)     3388 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/reason_no_timeframe.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/reason_no_timeframes.py
+-rw-r--r--   0 root         (0) root         (0)     2795 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/response_shipment.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/response_shipment_1.py
+-rw-r--r--   0 root         (0) root         (0)     3276 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/response_shipment_2.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/saturday.py
+-rw-r--r--   0 root         (0) root         (0)     1584 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/saturday_1.py
+-rw-r--r--   0 root         (0) root         (0)    18276 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment.py
+-rw-r--r--   0 root         (0) root         (0)    18866 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_1.py
+-rw-r--r--   0 root         (0) root         (0)     7281 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_11.py
+-rw-r--r--   0 root         (0) root         (0)     9494 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_2.py
+-rw-r--r--   0 root         (0) root         (0)      946 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_v_22_calculate_date_delivery_response.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_v_22_calculate_date_shipping_response.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shippingstatus_response.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shippingstatus_response_signature.py
+-rw-r--r--   0 root         (0) root         (0)     3451 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shippingstatus_response_updated_shipment.py
+-rw-r--r--   0 root         (0) root         (0)     2547 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/signature.py
+-rw-r--r--   0 root         (0) root         (0)     3380 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/status.py
+-rw-r--r--   0 root         (0) root         (0)     3360 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/status_2.py
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/string_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      809 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/string_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/sunday.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/sunday_1.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/sustainability.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/thursday.py
+-rw-r--r--   0 root         (0) root         (0)     1584 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/thursday_1.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe_1.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe_response.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe_timeframe.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframes.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframes_1.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/tuesday.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/tuesday_1.py
+-rw-r--r--   0 root         (0) root         (0)      532 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/type_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      850 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning_1.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning_11.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning_2.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warnings.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/wednesday.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/wednesday_1.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/postnlecommerce_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.921831 postnl_ecommerce_sdk-1.0.2/postnlecommerce/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/utilities/file_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)      732 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2024-05-01 14:28:03.924831 postnl_ecommerce_sdk-1.0.2/setup.cfg
```

### Comparing `postnl_ecommerce_sdk-1.0.1/LICENSE` & `postnl_ecommerce_sdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/PKG-INFO` & `postnl_ecommerce_sdk-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postnl-ecommerce-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Collection of PostNL API's for ecommerce processes.
 Author-email: PostNL <apimatic@postnl.nl>
 Project-URL: Documentation, https://developer.postnl.nl/docs
 Keywords: PostNL,SDK,API,ecommerce
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,58 +16,58 @@
 Requires-Dist: pytest>=7.2.2; extra == "testutils"
 
 
 # Getting Started with Postnl-Ecommerce
 
 ## Introduction
 
-<div><p><b>PostNL Ecommerce APIs</b></p><p>Explore our technical documentation, test your integration and go live with PostNL service.</p><p><b>Start using PostNL APIs for e-commerce processes</b></p><p>To get to know the PostNL APIs better, read all about it in our <a href='https://developer.postnl.nl/api-overview/'>API overview</a>. Learn everything you need to about our API's before embarking on integration with PostNL.</p><p>To connect to PostNL, you can request an API key via <a href='https://developer.postnl.nl/api-overview/'>Mijn PostNL</a> portal. Choose your APIs and build your integration. Explore our guides, examples, and resources to guide you through each phase of integration and start testing. Ensure that you can make successful test calls towards all endpoints used in the solution.</p><p>Contact our integrations team to have your test calls reviewed and gain access to our API production environment. Once everything is configured and validated, you'll be ready to go live and start using the PostNL service. <br>For help contact us via our support form: <a href='https://developer.postnl.nl/support/form/'>Need help? Submit a case | PostNL</a>.</p></div>
+<div><p><b>PostNL Ecommerce APIs</b></p><p>Explore our technical documentation, test your integration and go live with PostNL service.</p><p><b>Start using PostNL APIs for e-commerce processes</b></p><p>To get to know the PostNL APIs better, read all about it in our <a href='https://developer.postnl.nl/api-overview/'>API overview</a>. Learn everything you need to about our API's before embarking on integration with PostNL.</p><p>To connect to PostNL, you can request an API key via <a href='https://mijn.postnl.nl/c/BP2_Mod_Login.app?inresponseto=&RelayState=&startURL=%2F'>Mijn PostNL</a> portal. Choose your APIs and build your integration. Explore our guides, examples, and resources to guide you through each phase of integration and start testing. Ensure that you can make successful test calls towards all endpoints used in the solution.</p><p>Contact our integrations team to have your test calls reviewed and gain access to our API production environment. Once everything is configured and validated, you'll be ready to go live and start using the PostNL service.</p><p>For help contact us via our support form: <a href='https://developer.postnl.nl/support/form/'>Need help? Submit a case | PostNL</a>.</p></div>
 
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install postnl-ecommerce-sdk==1.0.1
+pip install postnl-ecommerce-sdk==1.0.2
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.1
+https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.2
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION_SERVER`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
 | `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
 | `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
 | `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
 | `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 3** |
 | `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
 | `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
 | `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
-| `custom_header_authentication_credentials` | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/custom-header-signature.md) | The credential object for Custom Header Signature |
+| `custom_header_authentication_credentials` | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md) | The credential object for Custom Header Signature |
 
 The API client can be initialized as follows:
 
 ```python
 client = PostnlecommerceClient(
     custom_header_authentication_credentials=CustomHeaderAuthenticationCredentials(
         apikey='apikey'
@@ -98,28 +98,28 @@
 | Production server | **Default** Production server |
 | Non-Production server | Sandbox environment for testing |
 
 ## Authorization
 
 This API uses the following authentication schemes.
 
-* [`APIKeyHeader (Custom Header Signature)`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/custom-header-signature.md)
+* [`APIKeyHeader (Custom Header Signature)`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md)
 
 ## List of APIs
 
-* [Postalcodecheck](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/postalcodecheck.md)
-* [Barcode](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/barcode.md)
-* [Checkout](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/checkout.md)
-* [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/confirming.md)
-* [Deliverydate](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/deliverydate.md)
-* [Labelling](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/labelling.md)
-* [Locations](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/locations.md)
-* [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/shipment.md)
-* [Shipping Status](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/shipping-status.md)
-* [Timeframes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/timeframes.md)
+* [Postalcodecheck](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/postalcodecheck.md)
+* [Barcode](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/barcode.md)
+* [Checkout](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/checkout.md)
+* [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/confirming.md)
+* [Deliverydate](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/deliverydate.md)
+* [Labelling](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/labelling.md)
+* [Locations](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/locations.md)
+* [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/shipment.md)
+* [Shipping Status](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/shipping-status.md)
+* [Timeframes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/timeframes.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/http-response.md)
-* [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/http-request.md)
+* [Utility Classes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-response.md)
+* [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-request.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: postnl-ecommerce-sdk Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: postnl-ecommerce-sdk Version: 1.0.2 Summary:
 Collection of PostNL API's for ecommerce processes. Author-email: PostNL
 postnl.nl> Project-URL: Documentation, https://developer.postnl.nl/docs
 Keywords: PostNL,SDK,API,ecommerce Requires-Python: >=3.7 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: apimatic-core~=0.2.0
 Requires-Dist: apimatic-core-interfaces~=0.1.0 Requires-Dist: apimatic-
 requests-client-adapter~=0.1.0 Requires-Dist: enum34>=1.1.10,~=1.1 Provides-
 Extra: testutils Requires-Dist: pytest>=7.2.2; extra == "testutils" # Getting
@@ -21,22 +21,22 @@
 the solution.
 Contact our integrations team to have your test calls reviewed and gain access
 to our API production environment. Once everything is configured and validated,
 you'll be ready to go live and start using the PostNL service.
 For help contact us via our support form: _N_e_e_d_ _h_e_l_p_?_ _S_u_b_m_i_t_ _a_ _c_a_s_e_ _|_ _P_o_s_t_N_L.
 ## Install the Package The package is compatible with Python versions `3 >=3.7,
 <= 3.11`. Install the package from PyPi using the following pip command:
-```python pip install postnl-ecommerce-sdk==1.0.1 ``` You can also view the
-package at: https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.1 ## Test the
+```python pip install postnl-ecommerce-sdk==1.0.2 ``` You can also view the
+package at: https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.2 ## Test the
 SDK You can test the generated SDK and the server with test cases. `unittest`
 is used as the testing framework and `pytest` is used as the test runner. You
 can run the tests as follows: Navigate to the root directory of the SDK and run
 the following commands ``` pip install -r test-requirements.txt pytest ``` ##
 Initialize the API Client **_Note:_** Documentation for the client can be found
-[here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/
+[here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/
 doc/client.md) The following parameters are configurable for the API Client: |
 Parameter | Type | Description | | --- | --- | --- | | `environment` |
 `Environment` | The API environment.
 **Default: `Environment.PRODUCTION_SERVER`** | | `http_client_instance` |
 `HttpClient` | The Http Client passed from the sdk user for making requests | |
 `override_http_client_configuration` | `bool` | The value which determines to
 override properties of the passed Http Client from the sdk user | |
@@ -50,16 +50,16 @@
 **Default: 2** | | `retry_statuses` | `Array of int` | The http statuses on
 which retry is to be done.
 **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** | |
 `retry_methods` | `Array of string` | The http methods on which retry is to be
 done.
 **Default: ['GET', 'PUT']** | | `custom_header_authentication_credentials` |
 [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.1/doc/$a/https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.1/custom-header-signature.md) | The credential
+ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-
+ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md) | The credential
 object for Custom Header Signature | The API client can be initialized as
 follows: ```python client = PostnlecommerceClient
 (
 custom_header_authentication_credentials=CustomHeaderAuthenticationCredentials
 ( apikey='apikey' ) ) ``` API calls return an `ApiResponse` object that
 includes the following fields: | Field | Description | | --- | --- | |
 `status_code` | Status code of the HTTP response | | `reason_phrase` | Reason
@@ -68,30 +68,30 @@
 | HTTP request info | | `errors` | Errors, if they exist | | `body` | The
 deserialized body of the HTTP response | ## Environments The SDK can be
 configured to use a different environment for making API calls. Available
 environments are: ### Fields | Name | Description | | --- | --- | | Production
 server | **Default** Production server | | Non-Production server | Sandbox
 environment for testing | ## Authorization This API uses the following
 authentication schemes. * [`APIKeyHeader (Custom Header Signature)`](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/$a/https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/custom-header-
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-
 signature.md) ## List of APIs * [Postalcodecheck](https://www.github.com/
-postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 postalcodecheck.md) * [Barcode](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.1/doc/controllers/barcode.md) * [Checkout](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+sdk-python/tree/1.0.2/doc/controllers/barcode.md) * [Checkout](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 checkout.md) * [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-
-python/tree/1.0.1/doc/controllers/confirming.md) * [Deliverydate](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+python/tree/1.0.2/doc/controllers/confirming.md) * [Deliverydate](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 deliverydate.md) * [Labelling](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.1/doc/controllers/labelling.md) * [Locations](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+sdk-python/tree/1.0.2/doc/controllers/labelling.md) * [Locations](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 locations.md) * [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-
-python/tree/1.0.1/doc/controllers/shipment.md) * [Shipping Status](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+python/tree/1.0.2/doc/controllers/shipment.md) * [Shipping Status](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 shipping-status.md) * [Timeframes](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.1/doc/controllers/timeframes.md) ## Classes
+ecommerce-sdk-python/tree/1.0.2/doc/controllers/timeframes.md) ## Classes
 Documentation * [Utility Classes](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.1/doc/utility-classes.md) * [HttpResponse](https:
-//www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/http-
+ecommerce-sdk-python/tree/1.0.2/doc/utility-classes.md) * [HttpResponse](https:
+//www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-
 response.md) * [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.1/doc/http-request.md)
+sdk-python/tree/1.0.2/doc/http-request.md)
```

### Comparing `postnl_ecommerce_sdk-1.0.1/README.md` & `postnl_ecommerce_sdk-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 
 # Getting Started with Postnl-Ecommerce
 
 ## Introduction
 
-<div><p><b>PostNL Ecommerce APIs</b></p><p>Explore our technical documentation, test your integration and go live with PostNL service.</p><p><b>Start using PostNL APIs for e-commerce processes</b></p><p>To get to know the PostNL APIs better, read all about it in our <a href='https://developer.postnl.nl/api-overview/'>API overview</a>. Learn everything you need to about our API's before embarking on integration with PostNL.</p><p>To connect to PostNL, you can request an API key via <a href='https://developer.postnl.nl/api-overview/'>Mijn PostNL</a> portal. Choose your APIs and build your integration. Explore our guides, examples, and resources to guide you through each phase of integration and start testing. Ensure that you can make successful test calls towards all endpoints used in the solution.</p><p>Contact our integrations team to have your test calls reviewed and gain access to our API production environment. Once everything is configured and validated, you'll be ready to go live and start using the PostNL service. <br>For help contact us via our support form: <a href='https://developer.postnl.nl/support/form/'>Need help? Submit a case | PostNL</a>.</p></div>
+<div><p><b>PostNL Ecommerce APIs</b></p><p>Explore our technical documentation, test your integration and go live with PostNL service.</p><p><b>Start using PostNL APIs for e-commerce processes</b></p><p>To get to know the PostNL APIs better, read all about it in our <a href='https://developer.postnl.nl/api-overview/'>API overview</a>. Learn everything you need to about our API's before embarking on integration with PostNL.</p><p>To connect to PostNL, you can request an API key via <a href='https://mijn.postnl.nl/c/BP2_Mod_Login.app?inresponseto=&RelayState=&startURL=%2F'>Mijn PostNL</a> portal. Choose your APIs and build your integration. Explore our guides, examples, and resources to guide you through each phase of integration and start testing. Ensure that you can make successful test calls towards all endpoints used in the solution.</p><p>Contact our integrations team to have your test calls reviewed and gain access to our API production environment. Once everything is configured and validated, you'll be ready to go live and start using the PostNL service.</p><p>For help contact us via our support form: <a href='https://developer.postnl.nl/support/form/'>Need help? Submit a case | PostNL</a>.</p></div>
 
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install postnl-ecommerce-sdk==1.0.1
+pip install postnl-ecommerce-sdk==1.0.2
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.1
+https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.2
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION_SERVER`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
 | `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
 | `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
 | `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
 | `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 3** |
 | `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
 | `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
 | `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
-| `custom_header_authentication_credentials` | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/custom-header-signature.md) | The credential object for Custom Header Signature |
+| `custom_header_authentication_credentials` | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md) | The credential object for Custom Header Signature |
 
 The API client can be initialized as follows:
 
 ```python
 client = PostnlecommerceClient(
     custom_header_authentication_credentials=CustomHeaderAuthenticationCredentials(
         apikey='apikey'
@@ -81,28 +81,28 @@
 | Production server | **Default** Production server |
 | Non-Production server | Sandbox environment for testing |
 
 ## Authorization
 
 This API uses the following authentication schemes.
 
-* [`APIKeyHeader (Custom Header Signature)`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/custom-header-signature.md)
+* [`APIKeyHeader (Custom Header Signature)`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md)
 
 ## List of APIs
 
-* [Postalcodecheck](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/postalcodecheck.md)
-* [Barcode](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/barcode.md)
-* [Checkout](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/checkout.md)
-* [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/confirming.md)
-* [Deliverydate](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/deliverydate.md)
-* [Labelling](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/labelling.md)
-* [Locations](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/locations.md)
-* [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/shipment.md)
-* [Shipping Status](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/shipping-status.md)
-* [Timeframes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/timeframes.md)
+* [Postalcodecheck](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/postalcodecheck.md)
+* [Barcode](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/barcode.md)
+* [Checkout](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/checkout.md)
+* [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/confirming.md)
+* [Deliverydate](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/deliverydate.md)
+* [Labelling](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/labelling.md)
+* [Locations](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/locations.md)
+* [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/shipment.md)
+* [Shipping Status](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/shipping-status.md)
+* [Timeframes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/timeframes.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/http-response.md)
-* [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/http-request.md)
+* [Utility Classes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-response.md)
+* [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-request.md)
```

#### html2text {}

```diff
@@ -13,22 +13,22 @@
 the solution.
 Contact our integrations team to have your test calls reviewed and gain access
 to our API production environment. Once everything is configured and validated,
 you'll be ready to go live and start using the PostNL service.
 For help contact us via our support form: _N_e_e_d_ _h_e_l_p_?_ _S_u_b_m_i_t_ _a_ _c_a_s_e_ _|_ _P_o_s_t_N_L.
 ## Install the Package The package is compatible with Python versions `3 >=3.7,
 <= 3.11`. Install the package from PyPi using the following pip command:
-```python pip install postnl-ecommerce-sdk==1.0.1 ``` You can also view the
-package at: https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.1 ## Test the
+```python pip install postnl-ecommerce-sdk==1.0.2 ``` You can also view the
+package at: https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.2 ## Test the
 SDK You can test the generated SDK and the server with test cases. `unittest`
 is used as the testing framework and `pytest` is used as the test runner. You
 can run the tests as follows: Navigate to the root directory of the SDK and run
 the following commands ``` pip install -r test-requirements.txt pytest ``` ##
 Initialize the API Client **_Note:_** Documentation for the client can be found
-[here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/
+[here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/
 doc/client.md) The following parameters are configurable for the API Client: |
 Parameter | Type | Description | | --- | --- | --- | | `environment` |
 `Environment` | The API environment.
 **Default: `Environment.PRODUCTION_SERVER`** | | `http_client_instance` |
 `HttpClient` | The Http Client passed from the sdk user for making requests | |
 `override_http_client_configuration` | `bool` | The value which determines to
 override properties of the passed Http Client from the sdk user | |
@@ -42,16 +42,16 @@
 **Default: 2** | | `retry_statuses` | `Array of int` | The http statuses on
 which retry is to be done.
 **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** | |
 `retry_methods` | `Array of string` | The http methods on which retry is to be
 done.
 **Default: ['GET', 'PUT']** | | `custom_header_authentication_credentials` |
 [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.1/doc/$a/https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.1/custom-header-signature.md) | The credential
+ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-
+ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md) | The credential
 object for Custom Header Signature | The API client can be initialized as
 follows: ```python client = PostnlecommerceClient
 (
 custom_header_authentication_credentials=CustomHeaderAuthenticationCredentials
 ( apikey='apikey' ) ) ``` API calls return an `ApiResponse` object that
 includes the following fields: | Field | Description | | --- | --- | |
 `status_code` | Status code of the HTTP response | | `reason_phrase` | Reason
@@ -60,30 +60,30 @@
 | HTTP request info | | `errors` | Errors, if they exist | | `body` | The
 deserialized body of the HTTP response | ## Environments The SDK can be
 configured to use a different environment for making API calls. Available
 environments are: ### Fields | Name | Description | | --- | --- | | Production
 server | **Default** Production server | | Non-Production server | Sandbox
 environment for testing | ## Authorization This API uses the following
 authentication schemes. * [`APIKeyHeader (Custom Header Signature)`](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/$a/https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/custom-header-
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-
 signature.md) ## List of APIs * [Postalcodecheck](https://www.github.com/
-postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 postalcodecheck.md) * [Barcode](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.1/doc/controllers/barcode.md) * [Checkout](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+sdk-python/tree/1.0.2/doc/controllers/barcode.md) * [Checkout](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 checkout.md) * [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-
-python/tree/1.0.1/doc/controllers/confirming.md) * [Deliverydate](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+python/tree/1.0.2/doc/controllers/confirming.md) * [Deliverydate](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 deliverydate.md) * [Labelling](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.1/doc/controllers/labelling.md) * [Locations](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+sdk-python/tree/1.0.2/doc/controllers/labelling.md) * [Locations](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 locations.md) * [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-
-python/tree/1.0.1/doc/controllers/shipment.md) * [Shipping Status](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+python/tree/1.0.2/doc/controllers/shipment.md) * [Shipping Status](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 shipping-status.md) * [Timeframes](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.1/doc/controllers/timeframes.md) ## Classes
+ecommerce-sdk-python/tree/1.0.2/doc/controllers/timeframes.md) ## Classes
 Documentation * [Utility Classes](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.1/doc/utility-classes.md) * [HttpResponse](https:
-//www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/http-
+ecommerce-sdk-python/tree/1.0.2/doc/utility-classes.md) * [HttpResponse](https:
+//www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-
 response.md) * [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.1/doc/http-request.md)
+sdk-python/tree/1.0.2/doc/http-request.md)
```

### Comparing `postnl_ecommerce_sdk-1.0.1/postnl_ecommerce_sdk.egg-info/PKG-INFO` & `postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postnl-ecommerce-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Collection of PostNL API's for ecommerce processes.
 Author-email: PostNL <apimatic@postnl.nl>
 Project-URL: Documentation, https://developer.postnl.nl/docs
 Keywords: PostNL,SDK,API,ecommerce
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,58 +16,58 @@
 Requires-Dist: pytest>=7.2.2; extra == "testutils"
 
 
 # Getting Started with Postnl-Ecommerce
 
 ## Introduction
 
-<div><p><b>PostNL Ecommerce APIs</b></p><p>Explore our technical documentation, test your integration and go live with PostNL service.</p><p><b>Start using PostNL APIs for e-commerce processes</b></p><p>To get to know the PostNL APIs better, read all about it in our <a href='https://developer.postnl.nl/api-overview/'>API overview</a>. Learn everything you need to about our API's before embarking on integration with PostNL.</p><p>To connect to PostNL, you can request an API key via <a href='https://developer.postnl.nl/api-overview/'>Mijn PostNL</a> portal. Choose your APIs and build your integration. Explore our guides, examples, and resources to guide you through each phase of integration and start testing. Ensure that you can make successful test calls towards all endpoints used in the solution.</p><p>Contact our integrations team to have your test calls reviewed and gain access to our API production environment. Once everything is configured and validated, you'll be ready to go live and start using the PostNL service. <br>For help contact us via our support form: <a href='https://developer.postnl.nl/support/form/'>Need help? Submit a case | PostNL</a>.</p></div>
+<div><p><b>PostNL Ecommerce APIs</b></p><p>Explore our technical documentation, test your integration and go live with PostNL service.</p><p><b>Start using PostNL APIs for e-commerce processes</b></p><p>To get to know the PostNL APIs better, read all about it in our <a href='https://developer.postnl.nl/api-overview/'>API overview</a>. Learn everything you need to about our API's before embarking on integration with PostNL.</p><p>To connect to PostNL, you can request an API key via <a href='https://mijn.postnl.nl/c/BP2_Mod_Login.app?inresponseto=&RelayState=&startURL=%2F'>Mijn PostNL</a> portal. Choose your APIs and build your integration. Explore our guides, examples, and resources to guide you through each phase of integration and start testing. Ensure that you can make successful test calls towards all endpoints used in the solution.</p><p>Contact our integrations team to have your test calls reviewed and gain access to our API production environment. Once everything is configured and validated, you'll be ready to go live and start using the PostNL service.</p><p>For help contact us via our support form: <a href='https://developer.postnl.nl/support/form/'>Need help? Submit a case | PostNL</a>.</p></div>
 
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install postnl-ecommerce-sdk==1.0.1
+pip install postnl-ecommerce-sdk==1.0.2
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.1
+https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.2
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION_SERVER`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
 | `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
 | `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
 | `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
 | `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 3** |
 | `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
 | `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
 | `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
-| `custom_header_authentication_credentials` | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/custom-header-signature.md) | The credential object for Custom Header Signature |
+| `custom_header_authentication_credentials` | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md) | The credential object for Custom Header Signature |
 
 The API client can be initialized as follows:
 
 ```python
 client = PostnlecommerceClient(
     custom_header_authentication_credentials=CustomHeaderAuthenticationCredentials(
         apikey='apikey'
@@ -98,28 +98,28 @@
 | Production server | **Default** Production server |
 | Non-Production server | Sandbox environment for testing |
 
 ## Authorization
 
 This API uses the following authentication schemes.
 
-* [`APIKeyHeader (Custom Header Signature)`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/custom-header-signature.md)
+* [`APIKeyHeader (Custom Header Signature)`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md)
 
 ## List of APIs
 
-* [Postalcodecheck](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/postalcodecheck.md)
-* [Barcode](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/barcode.md)
-* [Checkout](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/checkout.md)
-* [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/confirming.md)
-* [Deliverydate](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/deliverydate.md)
-* [Labelling](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/labelling.md)
-* [Locations](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/locations.md)
-* [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/shipment.md)
-* [Shipping Status](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/shipping-status.md)
-* [Timeframes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/timeframes.md)
+* [Postalcodecheck](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/postalcodecheck.md)
+* [Barcode](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/barcode.md)
+* [Checkout](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/checkout.md)
+* [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/confirming.md)
+* [Deliverydate](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/deliverydate.md)
+* [Labelling](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/labelling.md)
+* [Locations](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/locations.md)
+* [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/shipment.md)
+* [Shipping Status](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/shipping-status.md)
+* [Timeframes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/timeframes.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/http-response.md)
-* [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/http-request.md)
+* [Utility Classes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-response.md)
+* [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-request.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: postnl-ecommerce-sdk Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: postnl-ecommerce-sdk Version: 1.0.2 Summary:
 Collection of PostNL API's for ecommerce processes. Author-email: PostNL
 postnl.nl> Project-URL: Documentation, https://developer.postnl.nl/docs
 Keywords: PostNL,SDK,API,ecommerce Requires-Python: >=3.7 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: apimatic-core~=0.2.0
 Requires-Dist: apimatic-core-interfaces~=0.1.0 Requires-Dist: apimatic-
 requests-client-adapter~=0.1.0 Requires-Dist: enum34>=1.1.10,~=1.1 Provides-
 Extra: testutils Requires-Dist: pytest>=7.2.2; extra == "testutils" # Getting
@@ -21,22 +21,22 @@
 the solution.
 Contact our integrations team to have your test calls reviewed and gain access
 to our API production environment. Once everything is configured and validated,
 you'll be ready to go live and start using the PostNL service.
 For help contact us via our support form: _N_e_e_d_ _h_e_l_p_?_ _S_u_b_m_i_t_ _a_ _c_a_s_e_ _|_ _P_o_s_t_N_L.
 ## Install the Package The package is compatible with Python versions `3 >=3.7,
 <= 3.11`. Install the package from PyPi using the following pip command:
-```python pip install postnl-ecommerce-sdk==1.0.1 ``` You can also view the
-package at: https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.1 ## Test the
+```python pip install postnl-ecommerce-sdk==1.0.2 ``` You can also view the
+package at: https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.2 ## Test the
 SDK You can test the generated SDK and the server with test cases. `unittest`
 is used as the testing framework and `pytest` is used as the test runner. You
 can run the tests as follows: Navigate to the root directory of the SDK and run
 the following commands ``` pip install -r test-requirements.txt pytest ``` ##
 Initialize the API Client **_Note:_** Documentation for the client can be found
-[here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/
+[here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/
 doc/client.md) The following parameters are configurable for the API Client: |
 Parameter | Type | Description | | --- | --- | --- | | `environment` |
 `Environment` | The API environment.
 **Default: `Environment.PRODUCTION_SERVER`** | | `http_client_instance` |
 `HttpClient` | The Http Client passed from the sdk user for making requests | |
 `override_http_client_configuration` | `bool` | The value which determines to
 override properties of the passed Http Client from the sdk user | |
@@ -50,16 +50,16 @@
 **Default: 2** | | `retry_statuses` | `Array of int` | The http statuses on
 which retry is to be done.
 **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** | |
 `retry_methods` | `Array of string` | The http methods on which retry is to be
 done.
 **Default: ['GET', 'PUT']** | | `custom_header_authentication_credentials` |
 [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.1/doc/$a/https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.1/custom-header-signature.md) | The credential
+ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-
+ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md) | The credential
 object for Custom Header Signature | The API client can be initialized as
 follows: ```python client = PostnlecommerceClient
 (
 custom_header_authentication_credentials=CustomHeaderAuthenticationCredentials
 ( apikey='apikey' ) ) ``` API calls return an `ApiResponse` object that
 includes the following fields: | Field | Description | | --- | --- | |
 `status_code` | Status code of the HTTP response | | `reason_phrase` | Reason
@@ -68,30 +68,30 @@
 | HTTP request info | | `errors` | Errors, if they exist | | `body` | The
 deserialized body of the HTTP response | ## Environments The SDK can be
 configured to use a different environment for making API calls. Available
 environments are: ### Fields | Name | Description | | --- | --- | | Production
 server | **Default** Production server | | Non-Production server | Sandbox
 environment for testing | ## Authorization This API uses the following
 authentication schemes. * [`APIKeyHeader (Custom Header Signature)`](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/$a/https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/custom-header-
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-
 signature.md) ## List of APIs * [Postalcodecheck](https://www.github.com/
-postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 postalcodecheck.md) * [Barcode](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.1/doc/controllers/barcode.md) * [Checkout](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+sdk-python/tree/1.0.2/doc/controllers/barcode.md) * [Checkout](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 checkout.md) * [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-
-python/tree/1.0.1/doc/controllers/confirming.md) * [Deliverydate](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+python/tree/1.0.2/doc/controllers/confirming.md) * [Deliverydate](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 deliverydate.md) * [Labelling](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.1/doc/controllers/labelling.md) * [Locations](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+sdk-python/tree/1.0.2/doc/controllers/labelling.md) * [Locations](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 locations.md) * [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-
-python/tree/1.0.1/doc/controllers/shipment.md) * [Shipping Status](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/controllers/
+python/tree/1.0.2/doc/controllers/shipment.md) * [Shipping Status](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
 shipping-status.md) * [Timeframes](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.1/doc/controllers/timeframes.md) ## Classes
+ecommerce-sdk-python/tree/1.0.2/doc/controllers/timeframes.md) ## Classes
 Documentation * [Utility Classes](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.1/doc/utility-classes.md) * [HttpResponse](https:
-//www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.1/doc/http-
+ecommerce-sdk-python/tree/1.0.2/doc/utility-classes.md) * [HttpResponse](https:
+//www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-
 response.md) * [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.1/doc/http-request.md)
+sdk-python/tree/1.0.2/doc/http-request.md)
```

### Comparing `postnl_ecommerce_sdk-1.0.1/postnl_ecommerce_sdk.egg-info/SOURCES.txt` & `postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/api_helper.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/api_helper.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/configuration.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/configuration.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/barcode_controller.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/barcode_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/base_controller.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/checkout_controller.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/checkout_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/confirming_controller.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/confirming_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/deliverydate_controller.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/deliverydate_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/labelling_controller.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/labelling_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/locations_controller.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/locations_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/postalcode_check_controller.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/postalcode_check_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/shipment_controller.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/shipment_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/shipping_status_controller.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/shipping_status_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/controllers/timeframes_controller.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/timeframes_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/api_exception.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/barcode_method_not_allowed_exception.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_method_not_allowed_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/barcode_response_error_exception.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_response_error_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/barcode_response_invalid_exception.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/barcode_too_many_request_exception.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_too_many_request_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/checkout_response_invalid_exception.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/checkout_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/confirming_response_error_1_exception.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/confirming_response_error_1_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/deliverydate_response_invalid_exception.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/deliverydate_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/labelling_response_invalid_exception.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/labelling_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/locations_response_invalid_exception.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/locations_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/exceptions/timeframe_response_invalid_exception.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/timeframe_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/api_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/api_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/auth/custom_header_authentication.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/auth/custom_header_authentication.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/http_request.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/http_request.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/http/http_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/http_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/__init__.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/__init__.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address_11.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_11.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address_2.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_2.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address_3.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_3.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/address_4.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_4.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/amount.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/amount.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/amount_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/amount_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/barcode_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/barcode_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/checkout_request.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/checkout_request.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/checkout_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/checkout_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/code_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/code_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/complete_status.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/complete_status.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/confirming_request.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/confirming_request.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/confirming_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/confirming_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/contact.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/contact.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/content.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/content.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/content_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/content_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/cpc_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/cpc_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/currency_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/currency_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/current_status.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/current_status.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/custom.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/custom.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/customer.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/customer.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/customer_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/customer_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/customer_2.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/customer_2.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/cut_off_time.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/cut_off_time.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/day_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/day_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/delivery_option.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/delivery_option.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/delivery_options.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/delivery_options.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/detail.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/detail.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/dimension.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/dimension.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/dimension_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/dimension_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/error.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/error_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/error_2.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_2.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/error_3.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_3.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/error_4.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_4.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/event.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/event.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/expectation.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/expectation.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/extra_field.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/extra_field.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/fault.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/fault.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/friday.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/friday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/friday_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/friday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/get_locations_result.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/get_locations_result.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/get_locations_result_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/get_locations_result_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/group.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/group.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/hazardous_material.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/hazardous_material.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/label.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/label.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/label_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/label_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/labelling_request.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/labelling_request.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/labelling_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/labelling_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/labelling_response_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/labelling_response_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/language_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/language_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/location.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/location.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/location_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/location_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/location_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/location_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/locations_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/locations_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/merged_label.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/merged_label.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/message.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/message.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/message_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/message_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/monday.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/monday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/monday_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/monday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/old_status.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/old_status.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/opening_hours.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/opening_hours.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/option_1_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_1_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/option_2_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_2_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/option_3_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_3_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/option_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/options.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/options.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/options_2_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/options_2_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/pickup_option.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/pickup_option.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/product_option.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/product_option.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/product_option_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/product_option_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/product_options.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/product_options.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/reason_no_timeframe.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/reason_no_timeframe.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/reason_no_timeframes.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/reason_no_timeframes.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/response_shipment.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/response_shipment.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/response_shipment_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/response_shipment_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/response_shipment_2.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/response_shipment_2.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/saturday.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/saturday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/saturday_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/saturday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment_11.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_11.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment_2.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_2.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment_type_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_type_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment_v_22_calculate_date_delivery_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_v_22_calculate_date_delivery_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shipment_v_22_calculate_date_shipping_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_v_22_calculate_date_shipping_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shippingstatus_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shippingstatus_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shippingstatus_response_signature.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shippingstatus_response_signature.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/shippingstatus_response_updated_shipment.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shippingstatus_response_updated_shipment.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/signature.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/signature.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/status.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/status.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/status_2.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/status_2.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/string_1_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/string_1_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/string_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/string_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/sunday.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/sunday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/sunday_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/sunday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/sustainability.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/sustainability.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/thursday.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/thursday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/thursday_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/thursday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/timeframe.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/timeframe_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/timeframe_response.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/timeframe_timeframe.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe_timeframe.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/timeframes.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframes.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/timeframes_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframes_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/tuesday.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/tuesday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/tuesday_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/tuesday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/type_1_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/type_1_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/type_enum.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/type_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/warning.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/warning_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/warning_11.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning_11.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/warning_2.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning_2.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/warnings.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warnings.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/wednesday.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/wednesday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/models/wednesday_1.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/wednesday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/postnlecommerce/postnlecommerce_client.py` & `postnl_ecommerce_sdk-1.0.2/postnlecommerce/postnlecommerce_client.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.1/pyproject.toml` & `postnl_ecommerce_sdk-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "postnl-ecommerce-sdk"
 description = "Collection of PostNL API's for ecommerce processes."
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["PostNL", "SDK", "API", "ecommerce"]
 authors = [{name = "PostNL", email = "apimatic@postnl.nl"}]
 urls = {Documentation = "https://developer.postnl.nl/docs"}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "enum34~=1.1, >=1.1.10"]
 classifiers = []
```

