# ValidationsApiTagsV1UpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**is_public** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_tags_v1_update_request import ValidationsApiTagsV1UpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiTagsV1UpdateRequest from a JSON string
validations_api_tags_v1_update_request_instance = ValidationsApiTagsV1UpdateRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiTagsV1UpdateRequest.to_json())

# convert the object into a dict
validations_api_tags_v1_update_request_dict = validations_api_tags_v1_update_request_instance.to_dict()
# create an instance of ValidationsApiTagsV1UpdateRequest from a dict
validations_api_tags_v1_update_request_from_dict = ValidationsApiTagsV1UpdateRequest.from_dict(validations_api_tags_v1_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


