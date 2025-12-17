# edgraph_platform_client.CategoriesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_category_data_steward**](CategoriesApi.md#add_category_data_steward) | **POST** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/categories/{categoryId}/stewards | Adds a Data Steward to a Category.
[**add_category_data_steward_bulk**](CategoriesApi.md#add_category_data_steward_bulk) | **POST** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/categories/stewards | Adds a Data Steward to Categories.
[**certify_category**](CategoriesApi.md#certify_category) | **POST** /tenants/{tenantId}/statereporting/categories/{categoryId}/certify | Certifies a Category.
[**get_data_users_bulk**](CategoriesApi.md#get_data_users_bulk) | **GET** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/categories/datausers | Get all Data Users
[**get_state_reporting_categories**](CategoriesApi.md#get_state_reporting_categories) | **GET** /tenants/{tenantId}/statereporting/categories | Retrieves a list of Categories.
[**remove_category_data_owner**](CategoriesApi.md#remove_category_data_owner) | **DELETE** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/categories/{categoryId}/owner | Removes the Data Owner of a Category.
[**remove_category_data_steward**](CategoriesApi.md#remove_category_data_steward) | **DELETE** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/categories/{categoryId}/stewards/{email} | Removes a Data Steward from a Category.
[**request_category_certification_reminder**](CategoriesApi.md#request_category_certification_reminder) | **POST** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/categories/{categoryId}/certificationreminder | Requests a Certification Reminder to be sent.
[**set_category_data_owner**](CategoriesApi.md#set_category_data_owner) | **POST** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/categories/{categoryId}/owner | Sets the Data Owner of a Category.
[**set_category_data_owner_bulk**](CategoriesApi.md#set_category_data_owner_bulk) | **POST** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/categories/owner | Sets the Data Owner of Categories.
[**upload_state_reporting_category**](CategoriesApi.md#upload_state_reporting_category) | **POST** /tenants/{tenantId}/statereporting/categories/upload | Upload a Category via a JSON file.
[**upload_state_reporting_periods_from_category_json**](CategoriesApi.md#upload_state_reporting_periods_from_category_json) | **POST** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/upload | Upload a Category via a JSON file.


# **add_category_data_steward**
> ValidationsApiContainersV1DataStewardAddedResponse add_category_data_steward(tenant_id, category_id, reporting_period_id, validations_api_containers_v1_add_data_steward_request=validations_api_containers_v1_add_data_steward_request)

Adds a Data Steward to a Category.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_add_data_steward_request import ValidationsApiContainersV1AddDataStewardRequest
from edgraph_platform_client.models.validations_api_containers_v1_data_steward_added_response import ValidationsApiContainersV1DataStewardAddedResponse
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.CategoriesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    category_id = 'category_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    validations_api_containers_v1_add_data_steward_request = edgraph_platform_client.ValidationsApiContainersV1AddDataStewardRequest() # ValidationsApiContainersV1AddDataStewardRequest |  (optional)

    try:
        # Adds a Data Steward to a Category.
        api_response = api_instance.add_category_data_steward(tenant_id, category_id, reporting_period_id, validations_api_containers_v1_add_data_steward_request=validations_api_containers_v1_add_data_steward_request)
        print("The response of CategoriesApi->add_category_data_steward:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoriesApi->add_category_data_steward: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **category_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **validations_api_containers_v1_add_data_steward_request** | [**ValidationsApiContainersV1AddDataStewardRequest**](ValidationsApiContainersV1AddDataStewardRequest.md)|  | [optional] 

### Return type

[**ValidationsApiContainersV1DataStewardAddedResponse**](ValidationsApiContainersV1DataStewardAddedResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **add_category_data_steward_bulk**
> ValidationsApiContainersV1DataStewardAddedBulkResponse add_category_data_steward_bulk(tenant_id, reporting_period_id, validations_api_containers_v1_add_data_steward_bulk_request=validations_api_containers_v1_add_data_steward_bulk_request)

Adds a Data Steward to Categories.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_add_data_steward_bulk_request import ValidationsApiContainersV1AddDataStewardBulkRequest
from edgraph_platform_client.models.validations_api_containers_v1_data_steward_added_bulk_response import ValidationsApiContainersV1DataStewardAddedBulkResponse
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.CategoriesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    validations_api_containers_v1_add_data_steward_bulk_request = edgraph_platform_client.ValidationsApiContainersV1AddDataStewardBulkRequest() # ValidationsApiContainersV1AddDataStewardBulkRequest |  (optional)

    try:
        # Adds a Data Steward to Categories.
        api_response = api_instance.add_category_data_steward_bulk(tenant_id, reporting_period_id, validations_api_containers_v1_add_data_steward_bulk_request=validations_api_containers_v1_add_data_steward_bulk_request)
        print("The response of CategoriesApi->add_category_data_steward_bulk:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoriesApi->add_category_data_steward_bulk: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **validations_api_containers_v1_add_data_steward_bulk_request** | [**ValidationsApiContainersV1AddDataStewardBulkRequest**](ValidationsApiContainersV1AddDataStewardBulkRequest.md)|  | [optional] 

### Return type

[**ValidationsApiContainersV1DataStewardAddedBulkResponse**](ValidationsApiContainersV1DataStewardAddedBulkResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **certify_category**
> ValidationsApiContainersV1CertificationStatusSetResponse certify_category(tenant_id, category_id)

Certifies a Category.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_certification_status_set_response import ValidationsApiContainersV1CertificationStatusSetResponse
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.CategoriesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    category_id = 'category_id_example' # str | 

    try:
        # Certifies a Category.
        api_response = api_instance.certify_category(tenant_id, category_id)
        print("The response of CategoriesApi->certify_category:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoriesApi->certify_category: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **category_id** | **str**|  | 

### Return type

[**ValidationsApiContainersV1CertificationStatusSetResponse**](ValidationsApiContainersV1CertificationStatusSetResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_data_users_bulk**
> ValidationsApiContainersV1CategoriesWithDataUsersResponse get_data_users_bulk(tenant_id, reporting_period_id)

Get all Data Users

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_categories_with_data_users_response import ValidationsApiContainersV1CategoriesWithDataUsersResponse
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.CategoriesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 

    try:
        # Get all Data Users
        api_response = api_instance.get_data_users_bulk(tenant_id, reporting_period_id)
        print("The response of CategoriesApi->get_data_users_bulk:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoriesApi->get_data_users_bulk: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 

### Return type

[**ValidationsApiContainersV1CategoriesWithDataUsersResponse**](ValidationsApiContainersV1CategoriesWithDataUsersResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_state_reporting_categories**
> ValidationsApiContainersV1PaginatedContainers get_state_reporting_categories(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Retrieves a list of Categories.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_paginated_containers import ValidationsApiContainersV1PaginatedContainers
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.CategoriesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = '' # str |  (optional) (default to '')
    order_by = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Categories.
        api_response = api_instance.get_state_reporting_categories(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of CategoriesApi->get_state_reporting_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoriesApi->get_state_reporting_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**ValidationsApiContainersV1PaginatedContainers**](ValidationsApiContainersV1PaginatedContainers.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **remove_category_data_owner**
> remove_category_data_owner(tenant_id, reporting_period_id, category_id)

Removes the Data Owner of a Category.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.CategoriesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    category_id = 'category_id_example' # str | 

    try:
        # Removes the Data Owner of a Category.
        api_instance.remove_category_data_owner(tenant_id, reporting_period_id, category_id)
    except Exception as e:
        print("Exception when calling CategoriesApi->remove_category_data_owner: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **category_id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**204** | The resource was successfully deleted. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **remove_category_data_steward**
> remove_category_data_steward(tenant_id, category_id, reporting_period_id, email)

Removes a Data Steward from a Category.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.CategoriesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    category_id = 'category_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    email = 'email_example' # str | 

    try:
        # Removes a Data Steward from a Category.
        api_instance.remove_category_data_steward(tenant_id, category_id, reporting_period_id, email)
    except Exception as e:
        print("Exception when calling CategoriesApi->remove_category_data_steward: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **category_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **email** | **str**|  | 

### Return type

void (empty response body)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**204** | The resource was successfully deleted. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **request_category_certification_reminder**
> ValidationsApiContainersV1CertificationReminderRequestedResponse request_category_certification_reminder(tenant_id, reporting_period_id, category_id)

Requests a Certification Reminder to be sent.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_certification_reminder_requested_response import ValidationsApiContainersV1CertificationReminderRequestedResponse
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.CategoriesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    category_id = 'category_id_example' # str | 

    try:
        # Requests a Certification Reminder to be sent.
        api_response = api_instance.request_category_certification_reminder(tenant_id, reporting_period_id, category_id)
        print("The response of CategoriesApi->request_category_certification_reminder:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoriesApi->request_category_certification_reminder: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **category_id** | **str**|  | 

### Return type

[**ValidationsApiContainersV1CertificationReminderRequestedResponse**](ValidationsApiContainersV1CertificationReminderRequestedResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **set_category_data_owner**
> ValidationsApiContainersV1DataOwnerSetResponse set_category_data_owner(tenant_id, category_id, reporting_period_id, validations_api_containers_v1_set_data_owner_request=validations_api_containers_v1_set_data_owner_request)

Sets the Data Owner of a Category.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_data_owner_set_response import ValidationsApiContainersV1DataOwnerSetResponse
from edgraph_platform_client.models.validations_api_containers_v1_set_data_owner_request import ValidationsApiContainersV1SetDataOwnerRequest
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.CategoriesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    category_id = 'category_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    validations_api_containers_v1_set_data_owner_request = edgraph_platform_client.ValidationsApiContainersV1SetDataOwnerRequest() # ValidationsApiContainersV1SetDataOwnerRequest |  (optional)

    try:
        # Sets the Data Owner of a Category.
        api_response = api_instance.set_category_data_owner(tenant_id, category_id, reporting_period_id, validations_api_containers_v1_set_data_owner_request=validations_api_containers_v1_set_data_owner_request)
        print("The response of CategoriesApi->set_category_data_owner:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoriesApi->set_category_data_owner: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **category_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **validations_api_containers_v1_set_data_owner_request** | [**ValidationsApiContainersV1SetDataOwnerRequest**](ValidationsApiContainersV1SetDataOwnerRequest.md)|  | [optional] 

### Return type

[**ValidationsApiContainersV1DataOwnerSetResponse**](ValidationsApiContainersV1DataOwnerSetResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **set_category_data_owner_bulk**
> ValidationsApiContainersV1DataOwnerSetBulkResponse set_category_data_owner_bulk(tenant_id, reporting_period_id, validations_api_containers_v1_set_data_owner_bulk_request=validations_api_containers_v1_set_data_owner_bulk_request)

Sets the Data Owner of Categories.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_data_owner_set_bulk_response import ValidationsApiContainersV1DataOwnerSetBulkResponse
from edgraph_platform_client.models.validations_api_containers_v1_set_data_owner_bulk_request import ValidationsApiContainersV1SetDataOwnerBulkRequest
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.CategoriesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    validations_api_containers_v1_set_data_owner_bulk_request = edgraph_platform_client.ValidationsApiContainersV1SetDataOwnerBulkRequest() # ValidationsApiContainersV1SetDataOwnerBulkRequest |  (optional)

    try:
        # Sets the Data Owner of Categories.
        api_response = api_instance.set_category_data_owner_bulk(tenant_id, reporting_period_id, validations_api_containers_v1_set_data_owner_bulk_request=validations_api_containers_v1_set_data_owner_bulk_request)
        print("The response of CategoriesApi->set_category_data_owner_bulk:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoriesApi->set_category_data_owner_bulk: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **validations_api_containers_v1_set_data_owner_bulk_request** | [**ValidationsApiContainersV1SetDataOwnerBulkRequest**](ValidationsApiContainersV1SetDataOwnerBulkRequest.md)|  | [optional] 

### Return type

[**ValidationsApiContainersV1DataOwnerSetBulkResponse**](ValidationsApiContainersV1DataOwnerSetBulkResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upload_state_reporting_category**
> ValidationsApiContainersV1CollectionUploadedResponse upload_state_reporting_category(tenant_id, content_type=content_type, content_disposition=content_disposition, headers=headers, length=length, name=name, file_name=file_name)

Upload a Category via a JSON file.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_collection_uploaded_response import ValidationsApiContainersV1CollectionUploadedResponse
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.CategoriesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    content_type = 'content_type_example' # str |  (optional)
    content_disposition = 'content_disposition_example' # str |  (optional)
    headers = None # Dict[str, List[str]] |  (optional)
    length = 56 # int |  (optional)
    name = 'name_example' # str |  (optional)
    file_name = 'file_name_example' # str |  (optional)

    try:
        # Upload a Category via a JSON file.
        api_response = api_instance.upload_state_reporting_category(tenant_id, content_type=content_type, content_disposition=content_disposition, headers=headers, length=length, name=name, file_name=file_name)
        print("The response of CategoriesApi->upload_state_reporting_category:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoriesApi->upload_state_reporting_category: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **content_disposition** | **str**|  | [optional] 
 **headers** | [**Dict[str, List[str]]**](Dict.md)|  | [optional] 
 **length** | **int**|  | [optional] 
 **name** | **str**|  | [optional] 
 **file_name** | **str**|  | [optional] 

### Return type

[**ValidationsApiContainersV1CollectionUploadedResponse**](ValidationsApiContainersV1CollectionUploadedResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upload_state_reporting_periods_from_category_json**
> ValidationsApiContainersV1CollectionUploadedResponse upload_state_reporting_periods_from_category_json(tenant_id, environment_id, content_type=content_type, content_disposition=content_disposition, headers=headers, length=length, name=name, file_name=file_name)

Upload a Category via a JSON file.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_collection_uploaded_response import ValidationsApiContainersV1CollectionUploadedResponse
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.CategoriesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    content_type = 'content_type_example' # str |  (optional)
    content_disposition = 'content_disposition_example' # str |  (optional)
    headers = None # Dict[str, List[str]] |  (optional)
    length = 56 # int |  (optional)
    name = 'name_example' # str |  (optional)
    file_name = 'file_name_example' # str |  (optional)

    try:
        # Upload a Category via a JSON file.
        api_response = api_instance.upload_state_reporting_periods_from_category_json(tenant_id, environment_id, content_type=content_type, content_disposition=content_disposition, headers=headers, length=length, name=name, file_name=file_name)
        print("The response of CategoriesApi->upload_state_reporting_periods_from_category_json:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoriesApi->upload_state_reporting_periods_from_category_json: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **content_disposition** | **str**|  | [optional] 
 **headers** | [**Dict[str, List[str]]**](Dict.md)|  | [optional] 
 **length** | **int**|  | [optional] 
 **name** | **str**|  | [optional] 
 **file_name** | **str**|  | [optional] 

### Return type

[**ValidationsApiContainersV1CollectionUploadedResponse**](ValidationsApiContainersV1CollectionUploadedResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

