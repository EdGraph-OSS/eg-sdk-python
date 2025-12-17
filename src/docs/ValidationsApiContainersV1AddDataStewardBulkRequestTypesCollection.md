# ValidationsApiContainersV1AddDataStewardBulkRequestTypesCollection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**collection_id** | **str** |  | [optional] 
**stewards** | [**List[ValidationsApiContainersV1CollectionUser]**](ValidationsApiContainersV1CollectionUser.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_add_data_steward_bulk_request_types_collection import ValidationsApiContainersV1AddDataStewardBulkRequestTypesCollection

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1AddDataStewardBulkRequestTypesCollection from a JSON string
validations_api_containers_v1_add_data_steward_bulk_request_types_collection_instance = ValidationsApiContainersV1AddDataStewardBulkRequestTypesCollection.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1AddDataStewardBulkRequestTypesCollection.to_json())

# convert the object into a dict
validations_api_containers_v1_add_data_steward_bulk_request_types_collection_dict = validations_api_containers_v1_add_data_steward_bulk_request_types_collection_instance.to_dict()
# create an instance of ValidationsApiContainersV1AddDataStewardBulkRequestTypesCollection from a dict
validations_api_containers_v1_add_data_steward_bulk_request_types_collection_from_dict = ValidationsApiContainersV1AddDataStewardBulkRequestTypesCollection.from_dict(validations_api_containers_v1_add_data_steward_bulk_request_types_collection_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


