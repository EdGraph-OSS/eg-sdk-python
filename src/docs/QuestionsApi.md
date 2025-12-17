# edgraph_platform_client.QuestionsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_question**](QuestionsApi.md#create_question) | **POST** /tenants/{tenantId}/forms/{formId}/sections/{sectionId}/questions | Creates a new Question for a given section
[**delete_question**](QuestionsApi.md#delete_question) | **DELETE** /tenants/{tenantId}/forms/{formId}/sections/{sectionId}/questions/{questionId} | Deletes a Question.
[**get_question**](QuestionsApi.md#get_question) | **GET** /tenants/{tenantId}/forms/{formId}/sections/{sectionId}/questions/{questionId} | Get Question.
[**search_questions**](QuestionsApi.md#search_questions) | **GET** /tenants/{tenantId}/forms/{formId}/sections/{sectionId}/questions | Search Questions
[**update_question**](QuestionsApi.md#update_question) | **PUT** /tenants/{tenantId}/forms/{formId}/sections/{sectionId}/questions/{questionId} | Updates a Question.


# **create_question**
> FormApiQuestionsV1QuestionCreatedResponse create_question(tenant_id, form_id, section_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto)

Creates a new Question for a given section

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionRequestDto
from edgraph_platform_client.models.form_api_questions_v1_question_created_response import FormApiQuestionsV1QuestionCreatedResponse
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
    api_instance = edgraph_platform_client.QuestionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    section_id = 'section_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionRequestDto |  (optional)

    try:
        # Creates a new Question for a given section
        api_response = api_instance.create_question(tenant_id, form_id, section_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto)
        print("The response of QuestionsApi->create_question:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionsApi->create_question: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **section_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionRequestDto.md)|  | [optional] 

### Return type

[**FormApiQuestionsV1QuestionCreatedResponse**](FormApiQuestionsV1QuestionCreatedResponse.md)

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

# **delete_question**
> FormApiQuestionsV1QuestionDeletedResponse delete_question(tenant_id, form_id, section_id, question_id)

Deletes a Question.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_questions_v1_question_deleted_response import FormApiQuestionsV1QuestionDeletedResponse
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
    api_instance = edgraph_platform_client.QuestionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    section_id = 'section_id_example' # str | 
    question_id = 'question_id_example' # str | 

    try:
        # Deletes a Question.
        api_response = api_instance.delete_question(tenant_id, form_id, section_id, question_id)
        print("The response of QuestionsApi->delete_question:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionsApi->delete_question: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **section_id** | **str**|  | 
 **question_id** | **str**|  | 

### Return type

[**FormApiQuestionsV1QuestionDeletedResponse**](FormApiQuestionsV1QuestionDeletedResponse.md)

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

# **get_question**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionResponseDto get_question(tenant_id, form_id, section_id, question_id)

Get Question.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_forms_question_response_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionResponseDto
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
    api_instance = edgraph_platform_client.QuestionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    section_id = 'section_id_example' # str | 
    question_id = 'question_id_example' # str | 

    try:
        # Get Question.
        api_response = api_instance.get_question(tenant_id, form_id, section_id, question_id)
        print("The response of QuestionsApi->get_question:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionsApi->get_question: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **section_id** | **str**|  | 
 **question_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionResponseDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionResponseDto.md)

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

# **search_questions**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionResponseDtoPaginatedItemsViewModel search_questions(tenant_id, form_id, section_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Search Questions

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_forms_question_response_dto_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionResponseDtoPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.QuestionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    section_id = 'section_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Search Questions
        api_response = api_instance.search_questions(tenant_id, form_id, section_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of QuestionsApi->search_questions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionsApi->search_questions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **section_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionResponseDtoPaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionResponseDtoPaginatedItemsViewModel.md)

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

# **update_question**
> FormApiQuestionsV1QuestionUpdatedResponse update_question(tenant_id, form_id, section_id, question_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_update_question_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_update_question_request_dto)

Updates a Question.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_update_question_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsUpdateQuestionRequestDto
from edgraph_platform_client.models.form_api_questions_v1_question_updated_response import FormApiQuestionsV1QuestionUpdatedResponse
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
    api_instance = edgraph_platform_client.QuestionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    section_id = 'section_id_example' # str | 
    question_id = 'question_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_update_question_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsUpdateQuestionRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsUpdateQuestionRequestDto |  (optional)

    try:
        # Updates a Question.
        api_response = api_instance.update_question(tenant_id, form_id, section_id, question_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_update_question_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_update_question_request_dto)
        print("The response of QuestionsApi->update_question:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionsApi->update_question: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **section_id** | **str**|  | 
 **question_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_update_question_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsUpdateQuestionRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsUpdateQuestionRequestDto.md)|  | [optional] 

### Return type

[**FormApiQuestionsV1QuestionUpdatedResponse**](FormApiQuestionsV1QuestionUpdatedResponse.md)

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

