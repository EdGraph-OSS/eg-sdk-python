# ValidationsApiContainersV1UpdateCollectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**environment_type** | **str** |  | [optional] 
**tags** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_update_collection_request import ValidationsApiContainersV1UpdateCollectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1UpdateCollectionRequest from a JSON string
validations_api_containers_v1_update_collection_request_instance = ValidationsApiContainersV1UpdateCollectionRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1UpdateCollectionRequest.to_json())

# convert the object into a dict
validations_api_containers_v1_update_collection_request_dict = validations_api_containers_v1_update_collection_request_instance.to_dict()
# create an instance of ValidationsApiContainersV1UpdateCollectionRequest from a dict
validations_api_containers_v1_update_collection_request_from_dict = ValidationsApiContainersV1UpdateCollectionRequest.from_dict(validations_api_containers_v1_update_collection_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


