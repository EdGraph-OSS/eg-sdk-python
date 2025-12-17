# ValidationsApiContainersV1CollectionUploadedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**categories** | [**ValidationsApiContainersV1CollectionUploadedResponseTypesUploadResult**](ValidationsApiContainersV1CollectionUploadedResponseTypesUploadResult.md) |  | [optional] 
**sub_categories** | [**ValidationsApiContainersV1CollectionUploadedResponseTypesUploadResult**](ValidationsApiContainersV1CollectionUploadedResponseTypesUploadResult.md) |  | [optional] 
**rules** | [**ValidationsApiContainersV1CollectionUploadedResponseTypesUploadResult**](ValidationsApiContainersV1CollectionUploadedResponseTypesUploadResult.md) |  | [optional] 
**tags** | [**ValidationsApiContainersV1CollectionUploadedResponseTypesUploadResult**](ValidationsApiContainersV1CollectionUploadedResponseTypesUploadResult.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_collection_uploaded_response import ValidationsApiContainersV1CollectionUploadedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1CollectionUploadedResponse from a JSON string
validations_api_containers_v1_collection_uploaded_response_instance = ValidationsApiContainersV1CollectionUploadedResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1CollectionUploadedResponse.to_json())

# convert the object into a dict
validations_api_containers_v1_collection_uploaded_response_dict = validations_api_containers_v1_collection_uploaded_response_instance.to_dict()
# create an instance of ValidationsApiContainersV1CollectionUploadedResponse from a dict
validations_api_containers_v1_collection_uploaded_response_from_dict = ValidationsApiContainersV1CollectionUploadedResponse.from_dict(validations_api_containers_v1_collection_uploaded_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


