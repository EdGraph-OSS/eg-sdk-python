# ValidationsApiDbEnvironmentsV1PaginatedDbEnvironments


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ValidationsApiDbEnvironmentsV1DbEnvironmentDto]**](ValidationsApiDbEnvironmentsV1DbEnvironmentDto.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_db_environments_v1_paginated_db_environments import ValidationsApiDbEnvironmentsV1PaginatedDbEnvironments

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiDbEnvironmentsV1PaginatedDbEnvironments from a JSON string
validations_api_db_environments_v1_paginated_db_environments_instance = ValidationsApiDbEnvironmentsV1PaginatedDbEnvironments.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiDbEnvironmentsV1PaginatedDbEnvironments.to_json())

# convert the object into a dict
validations_api_db_environments_v1_paginated_db_environments_dict = validations_api_db_environments_v1_paginated_db_environments_instance.to_dict()
# create an instance of ValidationsApiDbEnvironmentsV1PaginatedDbEnvironments from a dict
validations_api_db_environments_v1_paginated_db_environments_from_dict = ValidationsApiDbEnvironmentsV1PaginatedDbEnvironments.from_dict(validations_api_db_environments_v1_paginated_db_environments_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


