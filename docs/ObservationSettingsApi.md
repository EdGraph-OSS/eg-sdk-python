# edgraph_platform_client.ObservationSettingsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_available_persona**](ObservationSettingsApi.md#add_available_persona) | **POST** /tenants/{tenantId}/observations/settings/personas | Adds a persona for a given Tenant
[**get_application_settings**](ObservationSettingsApi.md#get_application_settings) | **GET** /tenants/{tenantId}/observations/settings/application | Gets the application settings for the tenant
[**get_paginated_forms**](ObservationSettingsApi.md#get_paginated_forms) | **GET** /tenants/{tenantId}/observations/forms | Get Paginated Forms
[**get_paginated_personas**](ObservationSettingsApi.md#get_paginated_personas) | **GET** /tenants/{tenantId}/observations/settings/personas | Gets available personas
[**get_paginated_staff_classifications**](ObservationSettingsApi.md#get_paginated_staff_classifications) | **GET** /tenants/{tenantId}/observations/settings/available-staffclassifications | Get Paginated Available StaffClassifications
[**get_staff_classifications_settings**](ObservationSettingsApi.md#get_staff_classifications_settings) | **GET** /tenants/{tenantId}/observations/settings/staffclassifications | Gets the staffClassification settings for the tenant
[**set_application_settings**](ObservationSettingsApi.md#set_application_settings) | **POST** /tenants/{tenantId}/observations/settings/application | Sets the Application Settings of an Observation for a given Tenant
[**set_role_personas_settings**](ObservationSettingsApi.md#set_role_personas_settings) | **POST** /tenants/{tenantId}/observations/settings/rolepersonas | Updates personas assigned to a role configuration of the tenants setting
[**verify_sys_admin_credentials**](ObservationSettingsApi.md#verify_sys_admin_credentials) | **GET** /tenants/{tenantId}/observations/settings/verify-credentials | Gets the staffClassification settings for the tenant


# **add_available_persona**
> EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaResponse add_available_persona(tenant_id, ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request=ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request)

Adds a persona for a given Tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request import EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaRequest
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_response import EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaResponse
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
    api_instance = edgraph_platform_client.ObservationSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaRequest |  (optional)

    try:
        # Adds a persona for a given Tenant
        api_response = api_instance.add_available_persona(tenant_id, ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request=ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request)
        print("The response of ObservationSettingsApi->add_available_persona:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationSettingsApi->add_available_persona: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request** | [**EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaRequest**](EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaResponse.md)

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

# **get_application_settings**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetApplicationSettingsResponse get_application_settings(tenant_id)

Gets the application settings for the tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_application_settings_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetApplicationSettingsResponse
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
    api_instance = edgraph_platform_client.ObservationSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Gets the application settings for the tenant
        api_response = api_instance.get_application_settings(tenant_id)
        print("The response of ObservationSettingsApi->get_application_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationSettingsApi->get_application_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetApplicationSettingsResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetApplicationSettingsResponse.md)

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

# **get_paginated_forms**
> EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponseGetPaginatedItemsResponse get_paginated_forms(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Get Paginated Forms

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_form_response_get_paginated_items_response import EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponseGetPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ObservationSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Get Paginated Forms
        api_response = api_instance.get_paginated_forms(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of ObservationSettingsApi->get_paginated_forms:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationSettingsApi->get_paginated_forms: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponseGetPaginatedItemsResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponseGetPaginatedItemsResponse.md)

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

# **get_paginated_personas**
> EdGraphHttpAggregatorsTenantApiServicesObservationsPersonaResponseGetPaginatedItemsResponse get_paginated_personas(tenant_id)

Gets available personas

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_persona_response_get_paginated_items_response import EdGraphHttpAggregatorsTenantApiServicesObservationsPersonaResponseGetPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ObservationSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Gets available personas
        api_response = api_instance.get_paginated_personas(tenant_id)
        print("The response of ObservationSettingsApi->get_paginated_personas:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationSettingsApi->get_paginated_personas: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsPersonaResponseGetPaginatedItemsResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsPersonaResponseGetPaginatedItemsResponse.md)

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

# **get_paginated_staff_classifications**
> IdentityApiStaffClassificationV1GetStaffClassificationsResponse get_paginated_staff_classifications(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

Get Paginated Available StaffClassifications

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_staff_classification_v1_get_staff_classifications_response import IdentityApiStaffClassificationV1GetStaffClassificationsResponse
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
    api_instance = edgraph_platform_client.ObservationSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Get Paginated Available StaffClassifications
        api_response = api_instance.get_paginated_staff_classifications(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of ObservationSettingsApi->get_paginated_staff_classifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationSettingsApi->get_paginated_staff_classifications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IdentityApiStaffClassificationV1GetStaffClassificationsResponse**](IdentityApiStaffClassificationV1GetStaffClassificationsResponse.md)

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

# **get_staff_classifications_settings**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffClassificationSettingsResponse get_staff_classifications_settings(tenant_id)

Gets the staffClassification settings for the tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_staff_classification_settings_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffClassificationSettingsResponse
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
    api_instance = edgraph_platform_client.ObservationSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Gets the staffClassification settings for the tenant
        api_response = api_instance.get_staff_classifications_settings(tenant_id)
        print("The response of ObservationSettingsApi->get_staff_classifications_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationSettingsApi->get_staff_classifications_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffClassificationSettingsResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffClassificationSettingsResponse.md)

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

# **set_application_settings**
> EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsResponse set_application_settings(tenant_id, ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request=ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request)

Sets the Application Settings of an Observation for a given Tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request import EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsRequest
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_response import EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsResponse
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
    api_instance = edgraph_platform_client.ObservationSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsRequest |  (optional)

    try:
        # Sets the Application Settings of an Observation for a given Tenant
        api_response = api_instance.set_application_settings(tenant_id, ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request=ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request)
        print("The response of ObservationSettingsApi->set_application_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationSettingsApi->set_application_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request** | [**EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsRequest**](EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsResponse.md)

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

# **set_role_personas_settings**
> EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationResponse set_role_personas_settings(tenant_id, ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request=ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request)

Updates personas assigned to a role configuration of the tenants setting

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request import EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationRequest
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_response import EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationResponse
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
    api_instance = edgraph_platform_client.ObservationSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationRequest |  (optional)

    try:
        # Updates personas assigned to a role configuration of the tenants setting
        api_response = api_instance.set_role_personas_settings(tenant_id, ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request=ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request)
        print("The response of ObservationSettingsApi->set_role_personas_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationSettingsApi->set_role_personas_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request** | [**EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationRequest**](EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationResponse.md)

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

# **verify_sys_admin_credentials**
> object verify_sys_admin_credentials(tenant_id)

Gets the staffClassification settings for the tenant

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
    api_instance = edgraph_platform_client.ObservationSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Gets the staffClassification settings for the tenant
        api_response = api_instance.verify_sys_admin_credentials(tenant_id)
        print("The response of ObservationSettingsApi->verify_sys_admin_credentials:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationSettingsApi->verify_sys_admin_credentials: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

**object**

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

