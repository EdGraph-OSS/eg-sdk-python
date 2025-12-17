# ValidationsApiContainersV1DataUserResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**collection_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**data_owner** | [**ValidationsApiContainersV1CollectionUser**](ValidationsApiContainersV1CollectionUser.md) |  | [optional] 
**data_stewards** | [**List[ValidationsApiContainersV1CollectionUser]**](ValidationsApiContainersV1CollectionUser.md) |  | [optional] [readonly] 
**id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_data_user_response import ValidationsApiContainersV1DataUserResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1DataUserResponse from a JSON string
validations_api_containers_v1_data_user_response_instance = ValidationsApiContainersV1DataUserResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1DataUserResponse.to_json())

# convert the object into a dict
validations_api_containers_v1_data_user_response_dict = validations_api_containers_v1_data_user_response_instance.to_dict()
# create an instance of ValidationsApiContainersV1DataUserResponse from a dict
validations_api_containers_v1_data_user_response_from_dict = ValidationsApiContainersV1DataUserResponse.from_dict(validations_api_containers_v1_data_user_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


