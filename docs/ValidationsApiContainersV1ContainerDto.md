# ValidationsApiContainersV1ContainerDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**container_type** | **str** |  | [optional] 
**parent_container_id** | **str** |  | [optional] 
**is_default** | **bool** |  | [optional] 
**environment_type** | **str** |  | [optional] 
**child_containers** | [**List[ValidationsApiContainersV1ContainerDto]**](ValidationsApiContainersV1ContainerDto.md) |  | [optional] [readonly] 
**child_containers_count** | **int** |  | [optional] 
**tags** | [**List[ValidationsApiContainersV1ContainerDtoTypesTagDto]**](ValidationsApiContainersV1ContainerDtoTypesTagDto.md) |  | [optional] [readonly] 
**rules_count** | **int** |  | [optional] 
**certification_status** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_container_dto import ValidationsApiContainersV1ContainerDto

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1ContainerDto from a JSON string
validations_api_containers_v1_container_dto_instance = ValidationsApiContainersV1ContainerDto.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1ContainerDto.to_json())

# convert the object into a dict
validations_api_containers_v1_container_dto_dict = validations_api_containers_v1_container_dto_instance.to_dict()
# create an instance of ValidationsApiContainersV1ContainerDto from a dict
validations_api_containers_v1_container_dto_from_dict = ValidationsApiContainersV1ContainerDto.from_dict(validations_api_containers_v1_container_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


