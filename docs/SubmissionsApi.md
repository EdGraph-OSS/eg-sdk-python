# edgraph_platform_client.SubmissionsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_submission**](SubmissionsApi.md#create_submission) | **POST** /tenants/{tenantId}/forms/{formId}/submissions | Creates a new Submission for a given question
[**delete_submission**](SubmissionsApi.md#delete_submission) | **DELETE** /tenants/{tenantId}/forms/{formId}/submissions/{submissionId} | Deletes a Submission.
[**export_submissions**](SubmissionsApi.md#export_submissions) | **GET** /tenants/{tenantId}/forms/{formId}/submissions/export | Exports Submission data for a Form for a given tenant. (With JSON and CSV support)
[**get_submission**](SubmissionsApi.md#get_submission) | **GET** /tenants/{tenantId}/forms/{formId}/submissions/{submissionId} | Get Submission.
[**search_submissions**](SubmissionsApi.md#search_submissions) | **GET** /tenants/{tenantId}/forms/{formId}/submissions | Search Submissions
[**update_submission**](SubmissionsApi.md#update_submission) | **PUT** /tenants/{tenantId}/forms/{formId}/submissions/{submissionId} | Updates a Submission.


# **create_submission**
> FormApiSubmissionsV1SubmissionCreatedResponse create_submission(tenant_id, form_id, form_api_submissions_v1_create_submission_request=form_api_submissions_v1_create_submission_request)

Creates a new Submission for a given question

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_submissions_v1_create_submission_request import FormApiSubmissionsV1CreateSubmissionRequest
from edgraph_platform_client.models.form_api_submissions_v1_submission_created_response import FormApiSubmissionsV1SubmissionCreatedResponse
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
    api_instance = edgraph_platform_client.SubmissionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    form_api_submissions_v1_create_submission_request = edgraph_platform_client.FormApiSubmissionsV1CreateSubmissionRequest() # FormApiSubmissionsV1CreateSubmissionRequest |  (optional)

    try:
        # Creates a new Submission for a given question
        api_response = api_instance.create_submission(tenant_id, form_id, form_api_submissions_v1_create_submission_request=form_api_submissions_v1_create_submission_request)
        print("The response of SubmissionsApi->create_submission:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubmissionsApi->create_submission: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **form_api_submissions_v1_create_submission_request** | [**FormApiSubmissionsV1CreateSubmissionRequest**](FormApiSubmissionsV1CreateSubmissionRequest.md)|  | [optional] 

### Return type

[**FormApiSubmissionsV1SubmissionCreatedResponse**](FormApiSubmissionsV1SubmissionCreatedResponse.md)

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

# **delete_submission**
> FormApiSubmissionsV1SubmissionDeletedResponse delete_submission(tenant_id, form_id, submission_id)

Deletes a Submission.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_submissions_v1_submission_deleted_response import FormApiSubmissionsV1SubmissionDeletedResponse
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
    api_instance = edgraph_platform_client.SubmissionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    submission_id = 'submission_id_example' # str | 

    try:
        # Deletes a Submission.
        api_response = api_instance.delete_submission(tenant_id, form_id, submission_id)
        print("The response of SubmissionsApi->delete_submission:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubmissionsApi->delete_submission: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **submission_id** | **str**|  | 

### Return type

[**FormApiSubmissionsV1SubmissionDeletedResponse**](FormApiSubmissionsV1SubmissionDeletedResponse.md)

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

# **export_submissions**
> FormApiSubmissionsV1SubmissionsExportedResponse export_submissions(tenant_id, form_id, type=type)

Exports Submission data for a Form for a given tenant. (With JSON and CSV support)

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_submissions_v1_export_type import FormApiSubmissionsV1ExportType
from edgraph_platform_client.models.form_api_submissions_v1_submissions_exported_response import FormApiSubmissionsV1SubmissionsExportedResponse
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
    api_instance = edgraph_platform_client.SubmissionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    type = edgraph_platform_client.FormApiSubmissionsV1ExportType() # FormApiSubmissionsV1ExportType |  (optional)

    try:
        # Exports Submission data for a Form for a given tenant. (With JSON and CSV support)
        api_response = api_instance.export_submissions(tenant_id, form_id, type=type)
        print("The response of SubmissionsApi->export_submissions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubmissionsApi->export_submissions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **type** | [**FormApiSubmissionsV1ExportType**](.md)|  | [optional] 

### Return type

[**FormApiSubmissionsV1SubmissionsExportedResponse**](FormApiSubmissionsV1SubmissionsExportedResponse.md)

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

# **get_submission**
> FormApiSubmissionsV1SubmissionResponse get_submission(tenant_id, form_id, submission_id)

Get Submission.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_submissions_v1_submission_response import FormApiSubmissionsV1SubmissionResponse
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
    api_instance = edgraph_platform_client.SubmissionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    submission_id = 'submission_id_example' # str | 

    try:
        # Get Submission.
        api_response = api_instance.get_submission(tenant_id, form_id, submission_id)
        print("The response of SubmissionsApi->get_submission:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubmissionsApi->get_submission: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **submission_id** | **str**|  | 

### Return type

[**FormApiSubmissionsV1SubmissionResponse**](FormApiSubmissionsV1SubmissionResponse.md)

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

# **search_submissions**
> FormApiSubmissionsV1SubmissionResponsePaginatedItemsViewModel search_submissions(tenant_id, form_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Search Submissions

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_submissions_v1_submission_response_paginated_items_view_model import FormApiSubmissionsV1SubmissionResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.SubmissionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Search Submissions
        api_response = api_instance.search_submissions(tenant_id, form_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of SubmissionsApi->search_submissions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubmissionsApi->search_submissions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**FormApiSubmissionsV1SubmissionResponsePaginatedItemsViewModel**](FormApiSubmissionsV1SubmissionResponsePaginatedItemsViewModel.md)

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

# **update_submission**
> FormApiSubmissionsV1SubmissionUpdatedResponse update_submission(tenant_id, form_id, submission_id, form_api_submissions_v1_update_submission_request=form_api_submissions_v1_update_submission_request)

Updates a Submission.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_submissions_v1_submission_updated_response import FormApiSubmissionsV1SubmissionUpdatedResponse
from edgraph_platform_client.models.form_api_submissions_v1_update_submission_request import FormApiSubmissionsV1UpdateSubmissionRequest
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
    api_instance = edgraph_platform_client.SubmissionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    submission_id = 'submission_id_example' # str | 
    form_api_submissions_v1_update_submission_request = edgraph_platform_client.FormApiSubmissionsV1UpdateSubmissionRequest() # FormApiSubmissionsV1UpdateSubmissionRequest |  (optional)

    try:
        # Updates a Submission.
        api_response = api_instance.update_submission(tenant_id, form_id, submission_id, form_api_submissions_v1_update_submission_request=form_api_submissions_v1_update_submission_request)
        print("The response of SubmissionsApi->update_submission:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubmissionsApi->update_submission: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **submission_id** | **str**|  | 
 **form_api_submissions_v1_update_submission_request** | [**FormApiSubmissionsV1UpdateSubmissionRequest**](FormApiSubmissionsV1UpdateSubmissionRequest.md)|  | [optional] 

### Return type

[**FormApiSubmissionsV1SubmissionUpdatedResponse**](FormApiSubmissionsV1SubmissionUpdatedResponse.md)

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

