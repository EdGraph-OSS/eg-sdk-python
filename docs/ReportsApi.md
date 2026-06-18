# edgraph_platform_client.ReportsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_report_async**](ReportsApi.md#create_report_async) | **POST** /tenants/{tenantId}/analytics/reports | Creates a new report (Does not upload pbix file).
[**delete_report_async**](ReportsApi.md#delete_report_async) | **DELETE** /tenants/{tenantId}/analytics/reports/{reportId} | Removes a report.
[**download_report_async**](ReportsApi.md#download_report_async) | **GET** /tenants/{tenantId}/analytics/reports/download/{reportId}/{groupId} | Retrieves the PBIX for any report in the list in order to download
[**get_all_tenant_analytics_workspace_reports_async**](ReportsApi.md#get_all_tenant_analytics_workspace_reports_async) | **GET** /tenants/{tenantId}/analytics/reports | Retrieves all reports.
[**get_report_by_id_async**](ReportsApi.md#get_report_by_id_async) | **GET** /tenants/{tenantId}/analytics/reports/{reportId} | Retrieves a Report by ID.
[**sync_latest_version**](ReportsApi.md#sync_latest_version) | **POST** /tenants/{tenantId}/analytics/reports/synclatestversion | Sync latest version
[**sync_workspaces_async**](ReportsApi.md#sync_workspaces_async) | **POST** /tenants/{tenantId}/analytics/reports/sync | Triggers workspace, ODS and DW automation.
[**update_report_async**](ReportsApi.md#update_report_async) | **PUT** /tenants/{tenantId}/analytics/reports/{reportId} | Updates a report.


# **create_report_async**
> AnalyticsApiReportsV1ReportIdResponse create_report_async(tenant_id, file=file, name=name, short_description=short_description, description=description, tags=tags, is_visible=is_visible, version=version, identity_required=identity_required, roles_required=roles_required, state=state)

Creates a new report (Does not upload pbix file).

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_reports_v1_report_id_response import AnalyticsApiReportsV1ReportIdResponse
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
    api_instance = edgraph_platform_client.ReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    file = None # bytes |  (optional)
    name = 'name_example' # str |  (optional)
    short_description = 'short_description_example' # str |  (optional)
    description = 'description_example' # str |  (optional)
    tags = 'tags_example' # str |  (optional)
    is_visible = True # bool |  (optional)
    version = 'version_example' # str |  (optional)
    identity_required = True # bool |  (optional)
    roles_required = True # bool |  (optional)
    state = 'state_example' # str |  (optional)

    try:
        # Creates a new report (Does not upload pbix file).
        api_response = await api_instance.create_report_async(tenant_id, file=file, name=name, short_description=short_description, description=description, tags=tags, is_visible=is_visible, version=version, identity_required=identity_required, roles_required=roles_required, state=state)
        print("The response of ReportsApi->create_report_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->create_report_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **file** | **bytes**|  | [optional] 
 **name** | **str**|  | [optional] 
 **short_description** | **str**|  | [optional] 
 **description** | **str**|  | [optional] 
 **tags** | **str**|  | [optional] 
 **is_visible** | **bool**|  | [optional] 
 **version** | **str**|  | [optional] 
 **identity_required** | **bool**|  | [optional] 
 **roles_required** | **bool**|  | [optional] 
 **state** | **str**|  | [optional] 

### Return type

[**AnalyticsApiReportsV1ReportIdResponse**](AnalyticsApiReportsV1ReportIdResponse.md)

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_report_async**
> delete_report_async(tenant_id, report_id)

Removes a report.

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
    api_instance = edgraph_platform_client.ReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    report_id = 'report_id_example' # str | 

    try:
        # Removes a report.
        await api_instance.delete_report_async(tenant_id, report_id)
    except Exception as e:
        print("Exception when calling ReportsApi->delete_report_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **report_id** | **str**|  | 

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **download_report_async**
> AnalyticsApiReportsV1DownloadReportResponse download_report_async(tenant_id, report_id, group_id)

Retrieves the PBIX for any report in the list in order to download

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_reports_v1_download_report_response import AnalyticsApiReportsV1DownloadReportResponse
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
    api_instance = edgraph_platform_client.ReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    report_id = 'report_id_example' # str | 
    group_id = 'group_id_example' # str | 

    try:
        # Retrieves the PBIX for any report in the list in order to download
        api_response = await api_instance.download_report_async(tenant_id, report_id, group_id)
        print("The response of ReportsApi->download_report_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->download_report_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **report_id** | **str**|  | 
 **group_id** | **str**|  | 

### Return type

[**AnalyticsApiReportsV1DownloadReportResponse**](AnalyticsApiReportsV1DownloadReportResponse.md)

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

# **get_all_tenant_analytics_workspace_reports_async**
> AnalyticsApiReportsV1ReportPaginatedItemsResponse get_all_tenant_analytics_workspace_reports_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves all reports.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_reports_v1_report_paginated_items_response import AnalyticsApiReportsV1ReportPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves all reports.
        api_response = await api_instance.get_all_tenant_analytics_workspace_reports_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of ReportsApi->get_all_tenant_analytics_workspace_reports_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_all_tenant_analytics_workspace_reports_async: %s\n" % e)
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

[**AnalyticsApiReportsV1ReportPaginatedItemsResponse**](AnalyticsApiReportsV1ReportPaginatedItemsResponse.md)

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

# **get_report_by_id_async**
> AnalyticsApiReportsV1ReportResponse get_report_by_id_async(tenant_id, report_id)

Retrieves a Report by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_reports_v1_report_response import AnalyticsApiReportsV1ReportResponse
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
    api_instance = edgraph_platform_client.ReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    report_id = 'report_id_example' # str | 

    try:
        # Retrieves a Report by ID.
        api_response = await api_instance.get_report_by_id_async(tenant_id, report_id)
        print("The response of ReportsApi->get_report_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **report_id** | **str**|  | 

### Return type

[**AnalyticsApiReportsV1ReportResponse**](AnalyticsApiReportsV1ReportResponse.md)

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

# **sync_latest_version**
> object sync_latest_version(tenant_id, analytics_api_reports_v1_sync_latest_version_request=analytics_api_reports_v1_sync_latest_version_request)

Sync latest version

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_reports_v1_sync_latest_version_request import AnalyticsApiReportsV1SyncLatestVersionRequest
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
    api_instance = edgraph_platform_client.ReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    analytics_api_reports_v1_sync_latest_version_request = edgraph_platform_client.AnalyticsApiReportsV1SyncLatestVersionRequest() # AnalyticsApiReportsV1SyncLatestVersionRequest |  (optional)

    try:
        # Sync latest version
        api_response = await api_instance.sync_latest_version(tenant_id, analytics_api_reports_v1_sync_latest_version_request=analytics_api_reports_v1_sync_latest_version_request)
        print("The response of ReportsApi->sync_latest_version:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->sync_latest_version: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **analytics_api_reports_v1_sync_latest_version_request** | [**AnalyticsApiReportsV1SyncLatestVersionRequest**](AnalyticsApiReportsV1SyncLatestVersionRequest.md)|  | [optional] 

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sync_workspaces_async**
> object sync_workspaces_async(tenant_id, analytics_api_reports_v1_sync_workspaces_request=analytics_api_reports_v1_sync_workspaces_request)

Triggers workspace, ODS and DW automation.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_reports_v1_sync_workspaces_request import AnalyticsApiReportsV1SyncWorkspacesRequest
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
    api_instance = edgraph_platform_client.ReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    analytics_api_reports_v1_sync_workspaces_request = edgraph_platform_client.AnalyticsApiReportsV1SyncWorkspacesRequest() # AnalyticsApiReportsV1SyncWorkspacesRequest |  (optional)

    try:
        # Triggers workspace, ODS and DW automation.
        api_response = await api_instance.sync_workspaces_async(tenant_id, analytics_api_reports_v1_sync_workspaces_request=analytics_api_reports_v1_sync_workspaces_request)
        print("The response of ReportsApi->sync_workspaces_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->sync_workspaces_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **analytics_api_reports_v1_sync_workspaces_request** | [**AnalyticsApiReportsV1SyncWorkspacesRequest**](AnalyticsApiReportsV1SyncWorkspacesRequest.md)|  | [optional] 

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_report_async**
> AnalyticsApiReportsV1AnalyticsReport update_report_async(tenant_id, report_id, file=file, id=id, name=name, short_description=short_description, description=description, tags=tags, is_visible=is_visible, version=version, roles_required=roles_required, identity_required=identity_required, state=state)

Updates a report.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_reports_v1_analytics_report import AnalyticsApiReportsV1AnalyticsReport
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
    api_instance = edgraph_platform_client.ReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    report_id = 'report_id_example' # str | 
    file = None # bytes |  (optional)
    id = 'id_example' # str |  (optional)
    name = 'name_example' # str |  (optional)
    short_description = 'short_description_example' # str |  (optional)
    description = 'description_example' # str |  (optional)
    tags = 'tags_example' # str |  (optional)
    is_visible = True # bool |  (optional)
    version = 'version_example' # str |  (optional)
    roles_required = True # bool |  (optional)
    identity_required = True # bool |  (optional)
    state = 'state_example' # str |  (optional)

    try:
        # Updates a report.
        api_response = await api_instance.update_report_async(tenant_id, report_id, file=file, id=id, name=name, short_description=short_description, description=description, tags=tags, is_visible=is_visible, version=version, roles_required=roles_required, identity_required=identity_required, state=state)
        print("The response of ReportsApi->update_report_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->update_report_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **report_id** | **str**|  | 
 **file** | **bytes**|  | [optional] 
 **id** | **str**|  | [optional] 
 **name** | **str**|  | [optional] 
 **short_description** | **str**|  | [optional] 
 **description** | **str**|  | [optional] 
 **tags** | **str**|  | [optional] 
 **is_visible** | **bool**|  | [optional] 
 **version** | **str**|  | [optional] 
 **roles_required** | **bool**|  | [optional] 
 **identity_required** | **bool**|  | [optional] 
 **state** | **str**|  | [optional] 

### Return type

[**AnalyticsApiReportsV1AnalyticsReport**](AnalyticsApiReportsV1AnalyticsReport.md)

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

