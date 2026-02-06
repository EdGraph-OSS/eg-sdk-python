# edgraph_platform_client.InstancesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_related_instances**](InstancesApi.md#add_related_instances) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/relatedinstances | Add related instances to root instance by Id
[**add_school_year**](InstancesApi.md#add_school_year) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years | Adds an ODS database to an Instance.
[**add_school_year_range**](InstancesApi.md#add_school_year_range) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/bulk | Adds multiple ODS databases to an instance.
[**change_instance_database_tier_async**](InstancesApi.md#change_instance_database_tier_async) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/tiers | Changes the selected tier of an ODS database.
[**clone_instance_async**](InstancesApi.md#clone_instance_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/clone | Clones an instance.
[**create_instance**](InstancesApi.md#create_instance) | **POST** /tenants/{tenantId}/oneroster/instances | Creates a new Instance.
[**create_instance_async**](InstancesApi.md#create_instance_async) | **POST** /tenants/{tenantId}/edfiadmin/instances | Creates a new Instance.
[**delete_instance**](InstancesApi.md#delete_instance) | **DELETE** /tenants/{tenantId}/oneroster/instances/{instanceId} | Deletes an Instance.
[**delete_instance_async**](InstancesApi.md#delete_instance_async) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId} | Deletes an Instance.
[**delete_school_year_async**](InstancesApi.md#delete_school_year_async) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year} | Removes an ODS database from an Instance.
[**get_ed_fi_admin_instance_endpoints**](InstancesApi.md#get_ed_fi_admin_instance_endpoints) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/endpoints | Retrieves the Ed-Fi API endpoint URLs of an Instance.
[**get_ed_fi_admin_instance_year_endpoints**](InstancesApi.md#get_ed_fi_admin_instance_year_endpoints) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/endpoints | Retrieves the Ed-Fi API endpoint URLs of an Instance.
[**get_instance_by_id**](InstancesApi.md#get_instance_by_id) | **GET** /tenants/{tenantId}/oneroster/instances/{instanceId} | Retrieves an Instance by ID.
[**get_instance_by_id_async**](InstancesApi.md#get_instance_by_id_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId} | Retrieves an Instance by ID.
[**get_instance_csv_export**](InstancesApi.md#get_instance_csv_export) | **GET** /tenants/{tenantId}/oneroster/instances/{instanceId}/csv/export | Retrieves an Instance by ID.
[**get_instance_csv_export_v2**](InstancesApi.md#get_instance_csv_export_v2) | **GET** /v2/tenants/{tenantId}/oneroster/instances/{instanceId}/csv/export | Retrieves a ZIP bundle containing OneRoster Instance Database contents in CSV format
[**get_instance_endpoints**](InstancesApi.md#get_instance_endpoints) | **GET** /tenants/{tenantId}/oneroster/instances/{instanceId}/endpoints | Retrieves the One Roster endpoint URLs of an Instance.
[**get_instances_async**](InstancesApi.md#get_instances_async) | **GET** /tenants/{tenantId}/edfiadmin/instances | Retrieves a list of Instances.
[**get_paged_instances**](InstancesApi.md#get_paged_instances) | **GET** /tenants/{tenantId}/oneroster/instances | Retrieves a list of Instances.
[**get_tenant_instances_v2**](InstancesApi.md#get_tenant_instances_v2) | **GET** /v2/tenants/{tenantId}/instances | Get list of all instances for a tenant - V2
[**is_instance_custom_id_available**](InstancesApi.md#is_instance_custom_id_available) | **GET** /tenants/{tenantId}/oneroster/instances/isinstancecustomidavailable/{customId} | Validate if instance is available
[**load_api_metadata**](InstancesApi.md#load_api_metadata) | **POST** /tenants/{tenantId}/edfiadmin/api-metadata | Loads connection metadata.
[**reset_instance**](InstancesApi.md#reset_instance) | **POST** /tenants/{tenantId}/oneroster/instances/{instanceId}/resetinstance | Resets an Instance.
[**reset_instance_async**](InstancesApi.md#reset_instance_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/resetinstance | Resets an Instance.
[**reset_instance_cache_async**](InstancesApi.md#reset_instance_cache_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/resetcache | Resets the cache of an Instance and the specified ODS database.
[**reset_school_year_async**](InstancesApi.md#reset_school_year_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/resetods | Resets the ODS database with the specified school year.
[**set_instance_is_default**](InstancesApi.md#set_instance_is_default) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/default | Updates the isDefault property for an instance
[**test_connection_details_by_instance_id_async**](InstancesApi.md#test_connection_details_by_instance_id_async) | **POST** /tenants/{tenantId}/oneroster/instances/{instanceId}/test | Tests the connection by obtaining the details by Instance ID
[**test_credentials_connection**](InstancesApi.md#test_credentials_connection) | **POST** /tenants/{tenantId}/edfiadmin/testconnection | Tests availability of provided connection metadata.
[**test_instance_connection**](InstancesApi.md#test_instance_connection) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/testconnection | Tests the connection of the Instance.
[**test_instance_year_connection**](InstancesApi.md#test_instance_year_connection) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/testconnection | Tests the connection of the Instance.
[**truncate_instance**](InstancesApi.md#truncate_instance) | **POST** /tenants/{tenantId}/oneroster/instances/{instanceId}/truncate | Truncates the Instance&#39;s database
[**update_instance**](InstancesApi.md#update_instance) | **PUT** /tenants/{tenantId}/oneroster/instances/{instanceId} | Updates an Instance.
[**update_instance_async**](InstancesApi.md#update_instance_async) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId} | Updates an Instance.
[**validate_custom_id_available**](InstancesApi.md#validate_custom_id_available) | **GET** /tenants/{tenantId}/edfiadmin/instances/validatecustomidavailable/{customId} | Validate if instance is available


# **add_related_instances**
> EdfiAdminApiEdfiAdminV1AddRelatedInstancesResponse add_related_instances(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_add_related_instances_request=edfi_admin_api_edfi_admin_v1_add_related_instances_request)

Add related instances to root instance by Id

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_add_related_instances_request import EdfiAdminApiEdfiAdminV1AddRelatedInstancesRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_add_related_instances_response import EdfiAdminApiEdfiAdminV1AddRelatedInstancesResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_add_related_instances_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1AddRelatedInstancesRequest() # EdfiAdminApiEdfiAdminV1AddRelatedInstancesRequest |  (optional)

    try:
        # Add related instances to root instance by Id
        api_response = api_instance.add_related_instances(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_add_related_instances_request=edfi_admin_api_edfi_admin_v1_add_related_instances_request)
        print("The response of InstancesApi->add_related_instances:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->add_related_instances: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_add_related_instances_request** | [**EdfiAdminApiEdfiAdminV1AddRelatedInstancesRequest**](EdfiAdminApiEdfiAdminV1AddRelatedInstancesRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1AddRelatedInstancesResponse**](EdfiAdminApiEdfiAdminV1AddRelatedInstancesResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **add_school_year**
> add_school_year(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_add_school_year_request=edfi_admin_api_edfi_admin_v1_add_school_year_request)

Adds an ODS database to an Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_add_school_year_request import EdfiAdminApiEdfiAdminV1AddSchoolYearRequest
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_add_school_year_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1AddSchoolYearRequest() # EdfiAdminApiEdfiAdminV1AddSchoolYearRequest |  (optional)

    try:
        # Adds an ODS database to an Instance.
        api_instance.add_school_year(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_add_school_year_request=edfi_admin_api_edfi_admin_v1_add_school_year_request)
    except Exception as e:
        print("Exception when calling InstancesApi->add_school_year: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_add_school_year_request** | [**EdfiAdminApiEdfiAdminV1AddSchoolYearRequest**](EdfiAdminApiEdfiAdminV1AddSchoolYearRequest.md)|  | [optional] 

### Return type

void (empty response body)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **add_school_year_range**
> add_school_year_range(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_add_school_year_range_request=edfi_admin_api_edfi_admin_v1_add_school_year_range_request)

Adds multiple ODS databases to an instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_add_school_year_range_request import EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequest
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_add_school_year_range_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequest() # EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequest |  (optional)

    try:
        # Adds multiple ODS databases to an instance.
        api_instance.add_school_year_range(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_add_school_year_range_request=edfi_admin_api_edfi_admin_v1_add_school_year_range_request)
    except Exception as e:
        print("Exception when calling InstancesApi->add_school_year_range: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_add_school_year_range_request** | [**EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequest**](EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequest.md)|  | [optional] 

### Return type

void (empty response body)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **change_instance_database_tier_async**
> change_instance_database_tier_async(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_change_database_tier_request=edfi_admin_api_edfi_admin_v1_change_database_tier_request)

Changes the selected tier of an ODS database.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_change_database_tier_request import EdfiAdminApiEdfiAdminV1ChangeDatabaseTierRequest
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    edfi_admin_api_edfi_admin_v1_change_database_tier_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1ChangeDatabaseTierRequest() # EdfiAdminApiEdfiAdminV1ChangeDatabaseTierRequest |  (optional)

    try:
        # Changes the selected tier of an ODS database.
        api_instance.change_instance_database_tier_async(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_change_database_tier_request=edfi_admin_api_edfi_admin_v1_change_database_tier_request)
    except Exception as e:
        print("Exception when calling InstancesApi->change_instance_database_tier_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_change_database_tier_request** | [**EdfiAdminApiEdfiAdminV1ChangeDatabaseTierRequest**](EdfiAdminApiEdfiAdminV1ChangeDatabaseTierRequest.md)|  | [optional] 

### Return type

void (empty response body)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **clone_instance_async**
> EdfiAdminApiEdfiAdminV1CloneInstanceResponse clone_instance_async(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_clone_instance_request=edfi_admin_api_edfi_admin_v1_clone_instance_request)

Clones an instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_clone_instance_request import EdfiAdminApiEdfiAdminV1CloneInstanceRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_clone_instance_response import EdfiAdminApiEdfiAdminV1CloneInstanceResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_clone_instance_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1CloneInstanceRequest() # EdfiAdminApiEdfiAdminV1CloneInstanceRequest |  (optional)

    try:
        # Clones an instance.
        api_response = api_instance.clone_instance_async(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_clone_instance_request=edfi_admin_api_edfi_admin_v1_clone_instance_request)
        print("The response of InstancesApi->clone_instance_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->clone_instance_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_clone_instance_request** | [**EdfiAdminApiEdfiAdminV1CloneInstanceRequest**](EdfiAdminApiEdfiAdminV1CloneInstanceRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1CloneInstanceResponse**](EdfiAdminApiEdfiAdminV1CloneInstanceResponse.md)

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

# **create_instance**
> create_instance(tenant_id, ims_admin_api_v1_instances_create_instance_request=ims_admin_api_v1_instances_create_instance_request)

Creates a new Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_instances_create_instance_request import IMSAdminApiV1InstancesCreateInstanceRequest
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ims_admin_api_v1_instances_create_instance_request = edgraph_platform_client.IMSAdminApiV1InstancesCreateInstanceRequest() # IMSAdminApiV1InstancesCreateInstanceRequest |  (optional)

    try:
        # Creates a new Instance.
        api_instance.create_instance(tenant_id, ims_admin_api_v1_instances_create_instance_request=ims_admin_api_v1_instances_create_instance_request)
    except Exception as e:
        print("Exception when calling InstancesApi->create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ims_admin_api_v1_instances_create_instance_request** | [**IMSAdminApiV1InstancesCreateInstanceRequest**](IMSAdminApiV1InstancesCreateInstanceRequest.md)|  | [optional] 

### Return type

void (empty response body)

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
**200** | Success |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_instance_async**
> create_instance_async(tenant_id, edfi_admin_api_edfi_admin_v1_create_instance_request=edfi_admin_api_edfi_admin_v1_create_instance_request)

Creates a new Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_instance_request import EdfiAdminApiEdfiAdminV1CreateInstanceRequest
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_create_instance_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1CreateInstanceRequest() # EdfiAdminApiEdfiAdminV1CreateInstanceRequest |  (optional)

    try:
        # Creates a new Instance.
        api_instance.create_instance_async(tenant_id, edfi_admin_api_edfi_admin_v1_create_instance_request=edfi_admin_api_edfi_admin_v1_create_instance_request)
    except Exception as e:
        print("Exception when calling InstancesApi->create_instance_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_create_instance_request** | [**EdfiAdminApiEdfiAdminV1CreateInstanceRequest**](EdfiAdminApiEdfiAdminV1CreateInstanceRequest.md)|  | [optional] 

### Return type

void (empty response body)

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
**200** | Success |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_instance**
> delete_instance(tenant_id, instance_id)

Deletes an Instance.

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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Deletes an Instance.
        api_instance.delete_instance(tenant_id, instance_id)
    except Exception as e:
        print("Exception when calling InstancesApi->delete_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_instance_async**
> delete_instance_async(tenant_id, instance_id)

Deletes an Instance.

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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Deletes an Instance.
        api_instance.delete_instance_async(tenant_id, instance_id)
    except Exception as e:
        print("Exception when calling InstancesApi->delete_instance_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_school_year_async**
> delete_school_year_async(tenant_id, instance_id, year)

Removes an ODS database from an Instance.

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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 

    try:
        # Removes an ODS database from an Instance.
        api_instance.delete_school_year_async(tenant_id, instance_id, year)
    except Exception as e:
        print("Exception when calling InstancesApi->delete_school_year_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 

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
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_ed_fi_admin_instance_endpoints**
> EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse get_ed_fi_admin_instance_endpoints(tenant_id, instance_id)

Retrieves the Ed-Fi API endpoint URLs of an Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_endpoints_response import EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Retrieves the Ed-Fi API endpoint URLs of an Instance.
        api_response = api_instance.get_ed_fi_admin_instance_endpoints(tenant_id, instance_id)
        print("The response of InstancesApi->get_ed_fi_admin_instance_endpoints:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->get_ed_fi_admin_instance_endpoints: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse**](EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_ed_fi_admin_instance_year_endpoints**
> EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse get_ed_fi_admin_instance_year_endpoints(tenant_id, instance_id, year)

Retrieves the Ed-Fi API endpoint URLs of an Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_endpoints_response import EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 

    try:
        # Retrieves the Ed-Fi API endpoint URLs of an Instance.
        api_response = api_instance.get_ed_fi_admin_instance_year_endpoints(tenant_id, instance_id, year)
        print("The response of InstancesApi->get_ed_fi_admin_instance_year_endpoints:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->get_ed_fi_admin_instance_year_endpoints: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse**](EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_instance_by_id**
> IMSAdminApiV1InstancesInstanceProfileResponse get_instance_by_id(tenant_id, instance_id)

Retrieves an Instance by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_instances_instance_profile_response import IMSAdminApiV1InstancesInstanceProfileResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Retrieves an Instance by ID.
        api_response = api_instance.get_instance_by_id(tenant_id, instance_id)
        print("The response of InstancesApi->get_instance_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->get_instance_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

### Return type

[**IMSAdminApiV1InstancesInstanceProfileResponse**](IMSAdminApiV1InstancesInstanceProfileResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_instance_by_id_async**
> EdfiAdminApiEdfiAdminV1Instance get_instance_by_id_async(tenant_id, instance_id)

Retrieves an Instance by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance import EdfiAdminApiEdfiAdminV1Instance
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Retrieves an Instance by ID.
        api_response = api_instance.get_instance_by_id_async(tenant_id, instance_id)
        print("The response of InstancesApi->get_instance_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->get_instance_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1Instance**](EdfiAdminApiEdfiAdminV1Instance.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_instance_csv_export**
> IMSAdminApiV1InstancesGetInstanceCsvExportResponse get_instance_csv_export(tenant_id, instance_id)

Retrieves an Instance by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_instances_get_instance_csv_export_response import IMSAdminApiV1InstancesGetInstanceCsvExportResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Retrieves an Instance by ID.
        api_response = api_instance.get_instance_csv_export(tenant_id, instance_id)
        print("The response of InstancesApi->get_instance_csv_export:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->get_instance_csv_export: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

### Return type

[**IMSAdminApiV1InstancesGetInstanceCsvExportResponse**](IMSAdminApiV1InstancesGetInstanceCsvExportResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_instance_csv_export_v2**
> IMSAdminApiV1InstancesInstanceCsvExportedResponse get_instance_csv_export_v2(tenant_id, instance_id)

Retrieves a ZIP bundle containing OneRoster Instance Database contents in CSV format

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_instances_instance_csv_exported_response import IMSAdminApiV1InstancesInstanceCsvExportedResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Retrieves a ZIP bundle containing OneRoster Instance Database contents in CSV format
        api_response = api_instance.get_instance_csv_export_v2(tenant_id, instance_id)
        print("The response of InstancesApi->get_instance_csv_export_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->get_instance_csv_export_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

### Return type

[**IMSAdminApiV1InstancesInstanceCsvExportedResponse**](IMSAdminApiV1InstancesInstanceCsvExportedResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_instance_endpoints**
> IMSAdminApiV1InstancesInstanceEndpointsResponse get_instance_endpoints(tenant_id, instance_id)

Retrieves the One Roster endpoint URLs of an Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_instances_instance_endpoints_response import IMSAdminApiV1InstancesInstanceEndpointsResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Retrieves the One Roster endpoint URLs of an Instance.
        api_response = api_instance.get_instance_endpoints(tenant_id, instance_id)
        print("The response of InstancesApi->get_instance_endpoints:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->get_instance_endpoints: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

### Return type

[**IMSAdminApiV1InstancesInstanceEndpointsResponse**](IMSAdminApiV1InstancesInstanceEndpointsResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_instances_async**
> EdfiAdminApiEdfiAdminV1InstanceListModelPaginatedItemsViewModel get_instances_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter, deleted=deleted, target_tenant_id=target_tenant_id)

Retrieves a list of Instances.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_list_model_paginated_items_view_model import EdfiAdminApiEdfiAdminV1InstanceListModelPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')
    deleted = False # bool |  (optional) (default to False)
    target_tenant_id = 'target_tenant_id_example' # str |  (optional)

    try:
        # Retrieves a list of Instances.
        api_response = api_instance.get_instances_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter, deleted=deleted, target_tenant_id=target_tenant_id)
        print("The response of InstancesApi->get_instances_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->get_instances_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **deleted** | **bool**|  | [optional] [default to False]
 **target_tenant_id** | **str**|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceListModelPaginatedItemsViewModel**](EdfiAdminApiEdfiAdminV1InstanceListModelPaginatedItemsViewModel.md)

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

# **get_paged_instances**
> IMSAdminApiV1InstancesPagedInstancesResponse get_paged_instances(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of Instances.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_instances_paged_instances_response import IMSAdminApiV1InstancesPagedInstancesResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Instances.
        api_response = api_instance.get_paged_instances(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of InstancesApi->get_paged_instances:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->get_paged_instances: %s\n" % e)
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

[**IMSAdminApiV1InstancesPagedInstancesResponse**](IMSAdminApiV1InstancesPagedInstancesResponse.md)

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

# **get_tenant_instances_v2**
> EdGraphHttpAggregatorsTenantApiServicesInstancesInstanceResponsePaginatedItemsViewModel get_tenant_instances_v2(tenant_id, page_size=page_size, page_index=page_index, search_term=search_term, type=type)

Get list of all instances for a tenant - V2

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_instances_instance_response_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiServicesInstancesInstanceResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    search_term = '' # str |  (optional) (default to '')
    type = '' # str |  (optional) (default to '')

    try:
        # Get list of all instances for a tenant - V2
        api_response = api_instance.get_tenant_instances_v2(tenant_id, page_size=page_size, page_index=page_index, search_term=search_term, type=type)
        print("The response of InstancesApi->get_tenant_instances_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->get_tenant_instances_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **search_term** | **str**|  | [optional] [default to &#39;&#39;]
 **type** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesInstancesInstanceResponsePaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiServicesInstancesInstanceResponsePaginatedItemsViewModel.md)

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

# **is_instance_custom_id_available**
> bool is_instance_custom_id_available(tenant_id, custom_id)

Validate if instance is available

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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    custom_id = 'custom_id_example' # str | 

    try:
        # Validate if instance is available
        api_response = api_instance.is_instance_custom_id_available(tenant_id, custom_id)
        print("The response of InstancesApi->is_instance_custom_id_available:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->is_instance_custom_id_available: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **custom_id** | **str**|  | 

### Return type

**bool**

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

# **load_api_metadata**
> EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiLoadEdFiApiMetadataResult load_api_metadata(tenant_id, ed_graph_http_aggregators_tenant_api_services_onboarding_steps_ed_fi_api_metadata_request=ed_graph_http_aggregators_tenant_api_services_onboarding_steps_ed_fi_api_metadata_request)

Loads connection metadata.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_onboarding_steps_ed_fi_api_load_ed_fi_api_metadata_result import EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiLoadEdFiApiMetadataResult
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_onboarding_steps_ed_fi_api_metadata_request import EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiMetadataRequest
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_onboarding_steps_ed_fi_api_metadata_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiMetadataRequest() # EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiMetadataRequest |  (optional)

    try:
        # Loads connection metadata.
        api_response = api_instance.load_api_metadata(tenant_id, ed_graph_http_aggregators_tenant_api_services_onboarding_steps_ed_fi_api_metadata_request=ed_graph_http_aggregators_tenant_api_services_onboarding_steps_ed_fi_api_metadata_request)
        print("The response of InstancesApi->load_api_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->load_api_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_onboarding_steps_ed_fi_api_metadata_request** | [**EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiMetadataRequest**](EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiMetadataRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiLoadEdFiApiMetadataResult**](EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiLoadEdFiApiMetadataResult.md)

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

# **reset_instance**
> IMSAdminApiV1InstancesInstanceResetResponse reset_instance(tenant_id, instance_id)

Resets an Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_instances_instance_reset_response import IMSAdminApiV1InstancesInstanceResetResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Resets an Instance.
        api_response = api_instance.reset_instance(tenant_id, instance_id)
        print("The response of InstancesApi->reset_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->reset_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

### Return type

[**IMSAdminApiV1InstancesInstanceResetResponse**](IMSAdminApiV1InstancesInstanceResetResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reset_instance_async**
> EdfiAdminApiEdfiAdminV1ResetInstanceResponse reset_instance_async(tenant_id, instance_id)

Resets an Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_reset_instance_response import EdfiAdminApiEdfiAdminV1ResetInstanceResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Resets an Instance.
        api_response = api_instance.reset_instance_async(tenant_id, instance_id)
        print("The response of InstancesApi->reset_instance_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->reset_instance_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1ResetInstanceResponse**](EdfiAdminApiEdfiAdminV1ResetInstanceResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reset_instance_cache_async**
> EdfiAdminApiEdfiAdminV1ResetInstanceResponse reset_instance_cache_async(tenant_id, instance_id, year)

Resets the cache of an Instance and the specified ODS database.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_reset_instance_response import EdfiAdminApiEdfiAdminV1ResetInstanceResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 

    try:
        # Resets the cache of an Instance and the specified ODS database.
        api_response = api_instance.reset_instance_cache_async(tenant_id, instance_id, year)
        print("The response of InstancesApi->reset_instance_cache_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->reset_instance_cache_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1ResetInstanceResponse**](EdfiAdminApiEdfiAdminV1ResetInstanceResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reset_school_year_async**
> reset_school_year_async(tenant_id, instance_id, year)

Resets the ODS database with the specified school year.

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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 

    try:
        # Resets the ODS database with the specified school year.
        api_instance.reset_school_year_async(tenant_id, instance_id, year)
    except Exception as e:
        print("Exception when calling InstancesApi->reset_school_year_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 

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
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **set_instance_is_default**
> set_instance_is_default(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_set_instance_is_default_request=edfi_admin_api_edfi_admin_v1_set_instance_is_default_request)

Updates the isDefault property for an instance

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_set_instance_is_default_request import EdfiAdminApiEdfiAdminV1SetInstanceIsDefaultRequest
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_set_instance_is_default_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1SetInstanceIsDefaultRequest() # EdfiAdminApiEdfiAdminV1SetInstanceIsDefaultRequest |  (optional)

    try:
        # Updates the isDefault property for an instance
        api_instance.set_instance_is_default(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_set_instance_is_default_request=edfi_admin_api_edfi_admin_v1_set_instance_is_default_request)
    except Exception as e:
        print("Exception when calling InstancesApi->set_instance_is_default: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_set_instance_is_default_request** | [**EdfiAdminApiEdfiAdminV1SetInstanceIsDefaultRequest**](EdfiAdminApiEdfiAdminV1SetInstanceIsDefaultRequest.md)|  | [optional] 

### Return type

void (empty response body)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **test_connection_details_by_instance_id_async**
> IMSAdminApiV1ConnectionsConnectionTestedResponse test_connection_details_by_instance_id_async(tenant_id, instance_id, ims_admin_api_v1_connections_test_connection_details_by_instance_id_request=ims_admin_api_v1_connections_test_connection_details_by_instance_id_request)

Tests the connection by obtaining the details by Instance ID

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_connections_connection_tested_response import IMSAdminApiV1ConnectionsConnectionTestedResponse
from edgraph_platform_client.models.ims_admin_api_v1_connections_test_connection_details_by_instance_id_request import IMSAdminApiV1ConnectionsTestConnectionDetailsByInstanceIdRequest
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    ims_admin_api_v1_connections_test_connection_details_by_instance_id_request = edgraph_platform_client.IMSAdminApiV1ConnectionsTestConnectionDetailsByInstanceIdRequest() # IMSAdminApiV1ConnectionsTestConnectionDetailsByInstanceIdRequest |  (optional)

    try:
        # Tests the connection by obtaining the details by Instance ID
        api_response = api_instance.test_connection_details_by_instance_id_async(tenant_id, instance_id, ims_admin_api_v1_connections_test_connection_details_by_instance_id_request=ims_admin_api_v1_connections_test_connection_details_by_instance_id_request)
        print("The response of InstancesApi->test_connection_details_by_instance_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->test_connection_details_by_instance_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **ims_admin_api_v1_connections_test_connection_details_by_instance_id_request** | [**IMSAdminApiV1ConnectionsTestConnectionDetailsByInstanceIdRequest**](IMSAdminApiV1ConnectionsTestConnectionDetailsByInstanceIdRequest.md)|  | [optional] 

### Return type

[**IMSAdminApiV1ConnectionsConnectionTestedResponse**](IMSAdminApiV1ConnectionsConnectionTestedResponse.md)

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

# **test_credentials_connection**
> EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsTestConnectionResponse test_credentials_connection(tenant_id, body=body)

Tests availability of provided connection metadata.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_onboarding_steps_test_connection_response import EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsTestConnectionResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    body = None # object |  (optional)

    try:
        # Tests availability of provided connection metadata.
        api_response = api_instance.test_credentials_connection(tenant_id, body=body)
        print("The response of InstancesApi->test_credentials_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->test_credentials_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **body** | **object**|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsTestConnectionResponse**](EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsTestConnectionResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **test_instance_connection**
> EdfiAdminApiEdfiAdminV1TestInstanceConnectionResponse test_instance_connection(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_test_instance_connection_request=edfi_admin_api_edfi_admin_v1_test_instance_connection_request)

Tests the connection of the Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_test_instance_connection_request import EdfiAdminApiEdfiAdminV1TestInstanceConnectionRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_test_instance_connection_response import EdfiAdminApiEdfiAdminV1TestInstanceConnectionResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_test_instance_connection_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1TestInstanceConnectionRequest() # EdfiAdminApiEdfiAdminV1TestInstanceConnectionRequest |  (optional)

    try:
        # Tests the connection of the Instance.
        api_response = api_instance.test_instance_connection(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_test_instance_connection_request=edfi_admin_api_edfi_admin_v1_test_instance_connection_request)
        print("The response of InstancesApi->test_instance_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->test_instance_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_test_instance_connection_request** | [**EdfiAdminApiEdfiAdminV1TestInstanceConnectionRequest**](EdfiAdminApiEdfiAdminV1TestInstanceConnectionRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1TestInstanceConnectionResponse**](EdfiAdminApiEdfiAdminV1TestInstanceConnectionResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **test_instance_year_connection**
> EdfiAdminApiEdfiAdminV1TestInstanceConnectionResponse test_instance_year_connection(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_test_instance_connection_request=edfi_admin_api_edfi_admin_v1_test_instance_connection_request)

Tests the connection of the Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_test_instance_connection_request import EdfiAdminApiEdfiAdminV1TestInstanceConnectionRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_test_instance_connection_response import EdfiAdminApiEdfiAdminV1TestInstanceConnectionResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    edfi_admin_api_edfi_admin_v1_test_instance_connection_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1TestInstanceConnectionRequest() # EdfiAdminApiEdfiAdminV1TestInstanceConnectionRequest |  (optional)

    try:
        # Tests the connection of the Instance.
        api_response = api_instance.test_instance_year_connection(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_test_instance_connection_request=edfi_admin_api_edfi_admin_v1_test_instance_connection_request)
        print("The response of InstancesApi->test_instance_year_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->test_instance_year_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_test_instance_connection_request** | [**EdfiAdminApiEdfiAdminV1TestInstanceConnectionRequest**](EdfiAdminApiEdfiAdminV1TestInstanceConnectionRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1TestInstanceConnectionResponse**](EdfiAdminApiEdfiAdminV1TestInstanceConnectionResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **truncate_instance**
> IMSAdminApiV1InstancesInstanceTruncatedResponse truncate_instance(tenant_id, instance_id)

Truncates the Instance's database

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_instances_instance_truncated_response import IMSAdminApiV1InstancesInstanceTruncatedResponse
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Truncates the Instance's database
        api_response = api_instance.truncate_instance(tenant_id, instance_id)
        print("The response of InstancesApi->truncate_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->truncate_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

### Return type

[**IMSAdminApiV1InstancesInstanceTruncatedResponse**](IMSAdminApiV1InstancesInstanceTruncatedResponse.md)

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

# **update_instance**
> update_instance(tenant_id, instance_id, ims_admin_api_v1_instances_update_instance_request=ims_admin_api_v1_instances_update_instance_request)

Updates an Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_instances_update_instance_request import IMSAdminApiV1InstancesUpdateInstanceRequest
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    ims_admin_api_v1_instances_update_instance_request = edgraph_platform_client.IMSAdminApiV1InstancesUpdateInstanceRequest() # IMSAdminApiV1InstancesUpdateInstanceRequest |  (optional)

    try:
        # Updates an Instance.
        api_instance.update_instance(tenant_id, instance_id, ims_admin_api_v1_instances_update_instance_request=ims_admin_api_v1_instances_update_instance_request)
    except Exception as e:
        print("Exception when calling InstancesApi->update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **ims_admin_api_v1_instances_update_instance_request** | [**IMSAdminApiV1InstancesUpdateInstanceRequest**](IMSAdminApiV1InstancesUpdateInstanceRequest.md)|  | [optional] 

### Return type

void (empty response body)

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

# **update_instance_async**
> update_instance_async(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_update_instance_request=edfi_admin_api_edfi_admin_v1_update_instance_request)

Updates an Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_instance_request import EdfiAdminApiEdfiAdminV1UpdateInstanceRequest
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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_update_instance_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1UpdateInstanceRequest() # EdfiAdminApiEdfiAdminV1UpdateInstanceRequest |  (optional)

    try:
        # Updates an Instance.
        api_instance.update_instance_async(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_update_instance_request=edfi_admin_api_edfi_admin_v1_update_instance_request)
    except Exception as e:
        print("Exception when calling InstancesApi->update_instance_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_update_instance_request** | [**EdfiAdminApiEdfiAdminV1UpdateInstanceRequest**](EdfiAdminApiEdfiAdminV1UpdateInstanceRequest.md)|  | [optional] 

### Return type

void (empty response body)

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

# **validate_custom_id_available**
> bool validate_custom_id_available(tenant_id, custom_id)

Validate if instance is available

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
    api_instance = edgraph_platform_client.InstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    custom_id = 'custom_id_example' # str | 

    try:
        # Validate if instance is available
        api_response = api_instance.validate_custom_id_available(tenant_id, custom_id)
        print("The response of InstancesApi->validate_custom_id_available:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApi->validate_custom_id_available: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **custom_id** | **str**|  | 

### Return type

**bool**

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

