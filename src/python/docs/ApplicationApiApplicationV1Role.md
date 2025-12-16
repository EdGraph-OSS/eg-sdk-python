# ApplicationApiApplicationV1Role


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**role_name** | **str** |  | [optional] 
**is_default** | **bool** |  | [optional] 
**is_available_for_tenants** | **bool** |  | [optional] 
**display_name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**sort_order** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.application_api_application_v1_role import ApplicationApiApplicationV1Role

# TODO update the JSON string below
json = "{}"
# create an instance of ApplicationApiApplicationV1Role from a JSON string
application_api_application_v1_role_instance = ApplicationApiApplicationV1Role.from_json(json)
# print the JSON string representation of the object
print(ApplicationApiApplicationV1Role.to_json())

# convert the object into a dict
application_api_application_v1_role_dict = application_api_application_v1_role_instance.to_dict()
# create an instance of ApplicationApiApplicationV1Role from a dict
application_api_application_v1_role_from_dict = ApplicationApiApplicationV1Role.from_dict(application_api_application_v1_role_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


