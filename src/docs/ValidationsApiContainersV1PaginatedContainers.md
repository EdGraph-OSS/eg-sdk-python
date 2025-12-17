# ValidationsApiContainersV1PaginatedContainers


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ValidationsApiContainersV1ContainerDto]**](ValidationsApiContainersV1ContainerDto.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_paginated_containers import ValidationsApiContainersV1PaginatedContainers

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1PaginatedContainers from a JSON string
validations_api_containers_v1_paginated_containers_instance = ValidationsApiContainersV1PaginatedContainers.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1PaginatedContainers.to_json())

# convert the object into a dict
validations_api_containers_v1_paginated_containers_dict = validations_api_containers_v1_paginated_containers_instance.to_dict()
# create an instance of ValidationsApiContainersV1PaginatedContainers from a dict
validations_api_containers_v1_paginated_containers_from_dict = ValidationsApiContainersV1PaginatedContainers.from_dict(validations_api_containers_v1_paginated_containers_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


