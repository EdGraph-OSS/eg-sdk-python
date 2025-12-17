# ValidationsApiContainersV1SetDataOwnerRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**collection_id** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_set_data_owner_request import ValidationsApiContainersV1SetDataOwnerRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1SetDataOwnerRequest from a JSON string
validations_api_containers_v1_set_data_owner_request_instance = ValidationsApiContainersV1SetDataOwnerRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1SetDataOwnerRequest.to_json())

# convert the object into a dict
validations_api_containers_v1_set_data_owner_request_dict = validations_api_containers_v1_set_data_owner_request_instance.to_dict()
# create an instance of ValidationsApiContainersV1SetDataOwnerRequest from a dict
validations_api_containers_v1_set_data_owner_request_from_dict = ValidationsApiContainersV1SetDataOwnerRequest.from_dict(validations_api_containers_v1_set_data_owner_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


