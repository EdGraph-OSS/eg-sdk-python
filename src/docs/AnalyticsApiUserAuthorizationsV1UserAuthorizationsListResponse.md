# AnalyticsApiUserAuthorizationsV1UserAuthorizationsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**user_unique_id** | **str** |  | [optional] 
**user_email** | **str** |  | [optional] 
**user_type** | **str** |  | [optional] 
**user_role** | **str** |  | [optional] 
**source** | **str** |  | [optional] 
**authorized_scope** | **str** |  | [optional] 
**authorized_id** | **str** |  | [optional] 
**authorized_begin_date** | **str** |  | [optional] 
**authorized_end_date** | **str** |  | [optional] 
**school_year** | [**AnalyticsApiUserAuthorizationsV1SchoolYear**](AnalyticsApiUserAuthorizationsV1SchoolYear.md) |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_user_authorizations_v1_user_authorizations_list_response import AnalyticsApiUserAuthorizationsV1UserAuthorizationsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiUserAuthorizationsV1UserAuthorizationsListResponse from a JSON string
analytics_api_user_authorizations_v1_user_authorizations_list_response_instance = AnalyticsApiUserAuthorizationsV1UserAuthorizationsListResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiUserAuthorizationsV1UserAuthorizationsListResponse.to_json())

# convert the object into a dict
analytics_api_user_authorizations_v1_user_authorizations_list_response_dict = analytics_api_user_authorizations_v1_user_authorizations_list_response_instance.to_dict()
# create an instance of AnalyticsApiUserAuthorizationsV1UserAuthorizationsListResponse from a dict
analytics_api_user_authorizations_v1_user_authorizations_list_response_from_dict = AnalyticsApiUserAuthorizationsV1UserAuthorizationsListResponse.from_dict(analytics_api_user_authorizations_v1_user_authorizations_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


