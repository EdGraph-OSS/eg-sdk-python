# ValidationsApiContainersV1DataOwnerSetBulkResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**collections** | [**List[ValidationsApiContainersV1DataOwnerSetBulkResponseTypesCollection]**](ValidationsApiContainersV1DataOwnerSetBulkResponseTypesCollection.md) |  | [optional] [readonly] 
**reporting_period_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_data_owner_set_bulk_response import ValidationsApiContainersV1DataOwnerSetBulkResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1DataOwnerSetBulkResponse from a JSON string
validations_api_containers_v1_data_owner_set_bulk_response_instance = ValidationsApiContainersV1DataOwnerSetBulkResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1DataOwnerSetBulkResponse.to_json())

# convert the object into a dict
validations_api_containers_v1_data_owner_set_bulk_response_dict = validations_api_containers_v1_data_owner_set_bulk_response_instance.to_dict()
# create an instance of ValidationsApiContainersV1DataOwnerSetBulkResponse from a dict
validations_api_containers_v1_data_owner_set_bulk_response_from_dict = ValidationsApiContainersV1DataOwnerSetBulkResponse.from_dict(validations_api_containers_v1_data_owner_set_bulk_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


