# ApplicationApiApplicationV1ApplicationProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**application_type** | [**ApplicationApiApplicationV1ApplicationType**](ApplicationApiApplicationV1ApplicationType.md) |  | [optional] 
**application_name** | **str** |  | [optional] 
**application_uri** | **str** |  | [optional] 
**version** | **str** |  | [optional] 
**tooltip_text** | **str** |  | [optional] 
**application_description** | **str** |  | [optional] 
**tags** | **str** |  | [optional] 
**groups** | **str** |  | [optional] 
**application_status** | [**ApplicationApiApplicationV1ApplicationStatus**](ApplicationApiApplicationV1ApplicationStatus.md) |  | [optional] 
**open_in_new_window** | **bool** |  | [optional] 
**roles** | [**List[ApplicationApiApplicationV1Role]**](ApplicationApiApplicationV1Role.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**subscription_type** | [**ApplicationApiApplicationV1ApplicationSubscriptionType**](ApplicationApiApplicationV1ApplicationSubscriptionType.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.application_api_application_v1_application_profile_response import ApplicationApiApplicationV1ApplicationProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ApplicationApiApplicationV1ApplicationProfileResponse from a JSON string
application_api_application_v1_application_profile_response_instance = ApplicationApiApplicationV1ApplicationProfileResponse.from_json(json)
# print the JSON string representation of the object
print(ApplicationApiApplicationV1ApplicationProfileResponse.to_json())

# convert the object into a dict
application_api_application_v1_application_profile_response_dict = application_api_application_v1_application_profile_response_instance.to_dict()
# create an instance of ApplicationApiApplicationV1ApplicationProfileResponse from a dict
application_api_application_v1_application_profile_response_from_dict = ApplicationApiApplicationV1ApplicationProfileResponse.from_dict(application_api_application_v1_application_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


