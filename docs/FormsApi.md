# edgraph_platform_client.FormsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_form**](FormsApi.md#create_form) | **POST** /tenants/{tenantId}/forms | Creates a new Form for a given tenant
[**create_full_form**](FormsApi.md#create_full_form) | **POST** /tenants/{tenantId}/forms/full | Fully creates a new Form for a given tenant (with Sections and Questions).
[**delete_form**](FormsApi.md#delete_form) | **DELETE** /tenants/{tenantId}/forms/{formId} | Deletes a Form.
[**duplicate_form**](FormsApi.md#duplicate_form) | **POST** /tenants/{tenantId}/forms/{formId}/duplicate | Duplicates all Form data for a given tenant (with Sections and Questions).
[**get_form**](FormsApi.md#get_form) | **GET** /tenants/{tenantId}/forms/{formId} | Get Form.
[**get_form_access**](FormsApi.md#get_form_access) | **GET** /tenants/{tenantId}/forms/{formId}/access | Get the Access Type for a Form.
[**get_full_form_schema**](FormsApi.md#get_full_form_schema) | **GET** /tenants/{tenantId}/forms/{formId}/full/schemas | Get a Forms Json and UI React JSON compatible Schema.
[**import_form**](FormsApi.md#import_form) | **POST** /tenants/{tenantId}/forms/import | Imports all form data for a given tenant.
[**search_forms**](FormsApi.md#search_forms) | **GET** /tenants/{tenantId}/forms | Search Forms
[**set_form_access**](FormsApi.md#set_form_access) | **PUT** /tenants/{tenantId}/forms/{formId}/access | Sets the Access Type for a Form.
[**update_form**](FormsApi.md#update_form) | **PUT** /tenants/{tenantId}/forms/{formId} | Updates a Form.
[**update_full_form**](FormsApi.md#update_full_form) | **PUT** /tenants/{tenantId}/forms/{formId}/full | Fully updates a Form for a given tenant (with Sections and Questions).


# **create_form**
> FormApiFormsV1FormCreatedResponse create_form(tenant_id, form_api_forms_v1_create_form_request=form_api_forms_v1_create_form_request)

Creates a new Form for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_forms_v1_create_form_request import FormApiFormsV1CreateFormRequest
from edgraph_platform_client.models.form_api_forms_v1_form_created_response import FormApiFormsV1FormCreatedResponse
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.FormsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_api_forms_v1_create_form_request = edgraph_platform_client.FormApiFormsV1CreateFormRequest() # FormApiFormsV1CreateFormRequest |  (optional)

    try:
        # Creates a new Form for a given tenant
        api_response = await api_instance.create_form(tenant_id, form_api_forms_v1_create_form_request=form_api_forms_v1_create_form_request)
        print("The response of FormsApi->create_form:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormsApi->create_form: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_api_forms_v1_create_form_request** | [**FormApiFormsV1CreateFormRequest**](FormApiFormsV1CreateFormRequest.md)|  | [optional] 

### Return type

[**FormApiFormsV1FormCreatedResponse**](FormApiFormsV1FormCreatedResponse.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_full_form**
> FormApiFormsV1FullFormCreatedResponse create_full_form(tenant_id, form_api_forms_v1_create_full_form_request=form_api_forms_v1_create_full_form_request)

Fully creates a new Form for a given tenant (with Sections and Questions).

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_forms_v1_create_full_form_request import FormApiFormsV1CreateFullFormRequest
from edgraph_platform_client.models.form_api_forms_v1_full_form_created_response import FormApiFormsV1FullFormCreatedResponse
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.FormsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_api_forms_v1_create_full_form_request = edgraph_platform_client.FormApiFormsV1CreateFullFormRequest() # FormApiFormsV1CreateFullFormRequest |  (optional)

    try:
        # Fully creates a new Form for a given tenant (with Sections and Questions).
        api_response = await api_instance.create_full_form(tenant_id, form_api_forms_v1_create_full_form_request=form_api_forms_v1_create_full_form_request)
        print("The response of FormsApi->create_full_form:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormsApi->create_full_form: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_api_forms_v1_create_full_form_request** | [**FormApiFormsV1CreateFullFormRequest**](FormApiFormsV1CreateFullFormRequest.md)|  | [optional] 

### Return type

[**FormApiFormsV1FullFormCreatedResponse**](FormApiFormsV1FullFormCreatedResponse.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_form**
> FormApiFormsV1FormDeletedResponse delete_form(tenant_id, form_id)

Deletes a Form.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_forms_v1_form_deleted_response import FormApiFormsV1FormDeletedResponse
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.FormsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Deletes a Form.
        api_response = await api_instance.delete_form(tenant_id, form_id)
        print("The response of FormsApi->delete_form:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormsApi->delete_form: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 

### Return type

[**FormApiFormsV1FormDeletedResponse**](FormApiFormsV1FormDeletedResponse.md)

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

# **duplicate_form**
> FormApiFormsV1FormDuplicatedResponse duplicate_form(tenant_id, form_id)

Duplicates all Form data for a given tenant (with Sections and Questions).

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_forms_v1_form_duplicated_response import FormApiFormsV1FormDuplicatedResponse
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.FormsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Duplicates all Form data for a given tenant (with Sections and Questions).
        api_response = await api_instance.duplicate_form(tenant_id, form_id)
        print("The response of FormsApi->duplicate_form:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormsApi->duplicate_form: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 

### Return type

[**FormApiFormsV1FormDuplicatedResponse**](FormApiFormsV1FormDuplicatedResponse.md)

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

# **get_form**
> EdGraphHttpAggregatorsTenantApiServicesFormsV1Form get_form(tenant_id, form_id)

Get Form.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_forms_v1_form import EdGraphHttpAggregatorsTenantApiServicesFormsV1Form
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.FormsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Get Form.
        api_response = await api_instance.get_form(tenant_id, form_id)
        print("The response of FormsApi->get_form:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormsApi->get_form: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesFormsV1Form**](EdGraphHttpAggregatorsTenantApiServicesFormsV1Form.md)

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

# **get_form_access**
> FormApiFormsV1FormAccessResponse get_form_access(tenant_id, form_id)

Get the Access Type for a Form.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_forms_v1_form_access_response import FormApiFormsV1FormAccessResponse
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.FormsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Get the Access Type for a Form.
        api_response = await api_instance.get_form_access(tenant_id, form_id)
        print("The response of FormsApi->get_form_access:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormsApi->get_form_access: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 

### Return type

[**FormApiFormsV1FormAccessResponse**](FormApiFormsV1FormAccessResponse.md)

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

# **get_full_form_schema**
> FormApiFormsV1FullFormSchemaResponse get_full_form_schema(tenant_id, form_id)

Get a Forms Json and UI React JSON compatible Schema.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_forms_v1_full_form_schema_response import FormApiFormsV1FullFormSchemaResponse
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.FormsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Get a Forms Json and UI React JSON compatible Schema.
        api_response = await api_instance.get_full_form_schema(tenant_id, form_id)
        print("The response of FormsApi->get_full_form_schema:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormsApi->get_full_form_schema: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 

### Return type

[**FormApiFormsV1FullFormSchemaResponse**](FormApiFormsV1FullFormSchemaResponse.md)

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

# **import_form**
> object import_form(tenant_id, body=body)

Imports all form data for a given tenant.

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.FormsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    body = None # object |  (optional)

    try:
        # Imports all form data for a given tenant.
        api_response = await api_instance.import_form(tenant_id, body=body)
        print("The response of FormsApi->import_form:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormsApi->import_form: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **body** | **object**|  | [optional] 

### Return type

**object**

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **search_forms**
> EdGraphHttpAggregatorsTenantApiServicesFormsV1FormPaginatedItemsViewModel search_forms(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Search Forms

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_forms_v1_form_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiServicesFormsV1FormPaginatedItemsViewModel
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.FormsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Search Forms
        api_response = await api_instance.search_forms(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of FormsApi->search_forms:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormsApi->search_forms: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesFormsV1FormPaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiServicesFormsV1FormPaginatedItemsViewModel.md)

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

# **set_form_access**
> FormApiFormsV1FormAccessSetResponse set_form_access(tenant_id, form_id, form_api_forms_v1_set_form_access_request=form_api_forms_v1_set_form_access_request)

Sets the Access Type for a Form.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_forms_v1_form_access_set_response import FormApiFormsV1FormAccessSetResponse
from edgraph_platform_client.models.form_api_forms_v1_set_form_access_request import FormApiFormsV1SetFormAccessRequest
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.FormsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_api_forms_v1_set_form_access_request = edgraph_platform_client.FormApiFormsV1SetFormAccessRequest() # FormApiFormsV1SetFormAccessRequest |  (optional)

    try:
        # Sets the Access Type for a Form.
        api_response = await api_instance.set_form_access(tenant_id, form_id, form_api_forms_v1_set_form_access_request=form_api_forms_v1_set_form_access_request)
        print("The response of FormsApi->set_form_access:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormsApi->set_form_access: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 
 **form_api_forms_v1_set_form_access_request** | [**FormApiFormsV1SetFormAccessRequest**](FormApiFormsV1SetFormAccessRequest.md)|  | [optional] 

### Return type

[**FormApiFormsV1FormAccessSetResponse**](FormApiFormsV1FormAccessSetResponse.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_form**
> FormApiFormsV1FormUpdatedResponse update_form(tenant_id, form_id, form_api_forms_v1_update_form_request=form_api_forms_v1_update_form_request)

Updates a Form.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_forms_v1_form_updated_response import FormApiFormsV1FormUpdatedResponse
from edgraph_platform_client.models.form_api_forms_v1_update_form_request import FormApiFormsV1UpdateFormRequest
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.FormsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_api_forms_v1_update_form_request = edgraph_platform_client.FormApiFormsV1UpdateFormRequest() # FormApiFormsV1UpdateFormRequest |  (optional)

    try:
        # Updates a Form.
        api_response = await api_instance.update_form(tenant_id, form_id, form_api_forms_v1_update_form_request=form_api_forms_v1_update_form_request)
        print("The response of FormsApi->update_form:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormsApi->update_form: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 
 **form_api_forms_v1_update_form_request** | [**FormApiFormsV1UpdateFormRequest**](FormApiFormsV1UpdateFormRequest.md)|  | [optional] 

### Return type

[**FormApiFormsV1FormUpdatedResponse**](FormApiFormsV1FormUpdatedResponse.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_full_form**
> FormApiFormsV1FullFormUpdatedResponse update_full_form(tenant_id, form_id, form_api_forms_v1_update_full_form_request=form_api_forms_v1_update_full_form_request)

Fully updates a Form for a given tenant (with Sections and Questions).

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_forms_v1_full_form_updated_response import FormApiFormsV1FullFormUpdatedResponse
from edgraph_platform_client.models.form_api_forms_v1_update_full_form_request import FormApiFormsV1UpdateFullFormRequest
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.FormsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_api_forms_v1_update_full_form_request = edgraph_platform_client.FormApiFormsV1UpdateFullFormRequest() # FormApiFormsV1UpdateFullFormRequest |  (optional)

    try:
        # Fully updates a Form for a given tenant (with Sections and Questions).
        api_response = await api_instance.update_full_form(tenant_id, form_id, form_api_forms_v1_update_full_form_request=form_api_forms_v1_update_full_form_request)
        print("The response of FormsApi->update_full_form:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormsApi->update_full_form: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 
 **form_api_forms_v1_update_full_form_request** | [**FormApiFormsV1UpdateFullFormRequest**](FormApiFormsV1UpdateFullFormRequest.md)|  | [optional] 

### Return type

[**FormApiFormsV1FullFormUpdatedResponse**](FormApiFormsV1FullFormUpdatedResponse.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

