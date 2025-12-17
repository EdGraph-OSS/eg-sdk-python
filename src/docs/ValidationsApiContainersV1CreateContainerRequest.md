# ValidationsApiContainersV1CreateContainerRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**environment_type** | **str** |  | [optional] 
**tags** | **List[str]** |  | [optional] [readonly] 
**parent_container_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**urls** | [**List[ValidationsApiContainersV1Url]**](ValidationsApiContainersV1Url.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_create_container_request import ValidationsApiContainersV1CreateContainerRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1CreateContainerRequest from a JSON string
validations_api_containers_v1_create_container_request_instance = ValidationsApiContainersV1CreateContainerRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1CreateContainerRequest.to_json())

# convert the object into a dict
validations_api_containers_v1_create_container_request_dict = validations_api_containers_v1_create_container_request_instance.to_dict()
# create an instance of ValidationsApiContainersV1CreateContainerRequest from a dict
validations_api_containers_v1_create_container_request_from_dict = ValidationsApiContainersV1CreateContainerRequest.from_dict(validations_api_containers_v1_create_container_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


