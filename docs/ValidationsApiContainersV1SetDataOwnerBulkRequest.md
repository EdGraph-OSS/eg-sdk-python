# ValidationsApiContainersV1SetDataOwnerBulkRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**collections** | [**List[ValidationsApiContainersV1SetDataOwnerBulkRequestTypesCollection]**](ValidationsApiContainersV1SetDataOwnerBulkRequestTypesCollection.md) |  | [optional] [readonly] 
**reporting_period_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_set_data_owner_bulk_request import ValidationsApiContainersV1SetDataOwnerBulkRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1SetDataOwnerBulkRequest from a JSON string
validations_api_containers_v1_set_data_owner_bulk_request_instance = ValidationsApiContainersV1SetDataOwnerBulkRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1SetDataOwnerBulkRequest.to_json())

# convert the object into a dict
validations_api_containers_v1_set_data_owner_bulk_request_dict = validations_api_containers_v1_set_data_owner_bulk_request_instance.to_dict()
# create an instance of ValidationsApiContainersV1SetDataOwnerBulkRequest from a dict
validations_api_containers_v1_set_data_owner_bulk_request_from_dict = ValidationsApiContainersV1SetDataOwnerBulkRequest.from_dict(validations_api_containers_v1_set_data_owner_bulk_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


