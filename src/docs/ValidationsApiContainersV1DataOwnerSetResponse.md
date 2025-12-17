# ValidationsApiContainersV1DataOwnerSetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**collection_id** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_data_owner_set_response import ValidationsApiContainersV1DataOwnerSetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1DataOwnerSetResponse from a JSON string
validations_api_containers_v1_data_owner_set_response_instance = ValidationsApiContainersV1DataOwnerSetResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1DataOwnerSetResponse.to_json())

# convert the object into a dict
validations_api_containers_v1_data_owner_set_response_dict = validations_api_containers_v1_data_owner_set_response_instance.to_dict()
# create an instance of ValidationsApiContainersV1DataOwnerSetResponse from a dict
validations_api_containers_v1_data_owner_set_response_from_dict = ValidationsApiContainersV1DataOwnerSetResponse.from_dict(validations_api_containers_v1_data_owner_set_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


