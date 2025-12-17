# ValidationsApiContainersV1DataStewardAddedBulkResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**collections** | [**List[ValidationsApiContainersV1DataStewardAddedBulkResponseTypesCollection]**](ValidationsApiContainersV1DataStewardAddedBulkResponseTypesCollection.md) |  | [optional] [readonly] 
**reporting_period_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_data_steward_added_bulk_response import ValidationsApiContainersV1DataStewardAddedBulkResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1DataStewardAddedBulkResponse from a JSON string
validations_api_containers_v1_data_steward_added_bulk_response_instance = ValidationsApiContainersV1DataStewardAddedBulkResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1DataStewardAddedBulkResponse.to_json())

# convert the object into a dict
validations_api_containers_v1_data_steward_added_bulk_response_dict = validations_api_containers_v1_data_steward_added_bulk_response_instance.to_dict()
# create an instance of ValidationsApiContainersV1DataStewardAddedBulkResponse from a dict
validations_api_containers_v1_data_steward_added_bulk_response_from_dict = ValidationsApiContainersV1DataStewardAddedBulkResponse.from_dict(validations_api_containers_v1_data_steward_added_bulk_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


