# ValidationsApiContainersV1UploadCollectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**collection_json** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_upload_collection_request import ValidationsApiContainersV1UploadCollectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1UploadCollectionRequest from a JSON string
validations_api_containers_v1_upload_collection_request_instance = ValidationsApiContainersV1UploadCollectionRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1UploadCollectionRequest.to_json())

# convert the object into a dict
validations_api_containers_v1_upload_collection_request_dict = validations_api_containers_v1_upload_collection_request_instance.to_dict()
# create an instance of ValidationsApiContainersV1UploadCollectionRequest from a dict
validations_api_containers_v1_upload_collection_request_from_dict = ValidationsApiContainersV1UploadCollectionRequest.from_dict(validations_api_containers_v1_upload_collection_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


