# AnalyticsApiUserAuthorizationsV1UserAuthorizationsPaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[AnalyticsApiUserAuthorizationsV1UserAuthorizationsListResponse]**](AnalyticsApiUserAuthorizationsV1UserAuthorizationsListResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.analytics_api_user_authorizations_v1_user_authorizations_paginated_items_response import AnalyticsApiUserAuthorizationsV1UserAuthorizationsPaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiUserAuthorizationsV1UserAuthorizationsPaginatedItemsResponse from a JSON string
analytics_api_user_authorizations_v1_user_authorizations_paginated_items_response_instance = AnalyticsApiUserAuthorizationsV1UserAuthorizationsPaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiUserAuthorizationsV1UserAuthorizationsPaginatedItemsResponse.to_json())

# convert the object into a dict
analytics_api_user_authorizations_v1_user_authorizations_paginated_items_response_dict = analytics_api_user_authorizations_v1_user_authorizations_paginated_items_response_instance.to_dict()
# create an instance of AnalyticsApiUserAuthorizationsV1UserAuthorizationsPaginatedItemsResponse from a dict
analytics_api_user_authorizations_v1_user_authorizations_paginated_items_response_from_dict = AnalyticsApiUserAuthorizationsV1UserAuthorizationsPaginatedItemsResponse.from_dict(analytics_api_user_authorizations_v1_user_authorizations_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


