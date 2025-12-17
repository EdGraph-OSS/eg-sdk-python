# ApplicationApiApplicationV1ApplicationListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**application_name** | **str** |  | [optional] 
**version** | **str** |  | [optional] 
**tags** | **str** |  | [optional] 
**groups** | **str** |  | [optional] 
**application_status** | [**ApplicationApiApplicationV1ApplicationStatus**](ApplicationApiApplicationV1ApplicationStatus.md) |  | [optional] 
**roles** | [**List[ApplicationApiApplicationV1Role]**](ApplicationApiApplicationV1Role.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_at** | **str** |  | [optional] 
**subscription_type** | [**ApplicationApiApplicationV1ApplicationSubscriptionType**](ApplicationApiApplicationV1ApplicationSubscriptionType.md) |  | [optional] 
**documentation_url** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.application_api_application_v1_application_list_response import ApplicationApiApplicationV1ApplicationListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ApplicationApiApplicationV1ApplicationListResponse from a JSON string
application_api_application_v1_application_list_response_instance = ApplicationApiApplicationV1ApplicationListResponse.from_json(json)
# print the JSON string representation of the object
print(ApplicationApiApplicationV1ApplicationListResponse.to_json())

# convert the object into a dict
application_api_application_v1_application_list_response_dict = application_api_application_v1_application_list_response_instance.to_dict()
# create an instance of ApplicationApiApplicationV1ApplicationListResponse from a dict
application_api_application_v1_application_list_response_from_dict = ApplicationApiApplicationV1ApplicationListResponse.from_dict(application_api_application_v1_application_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


