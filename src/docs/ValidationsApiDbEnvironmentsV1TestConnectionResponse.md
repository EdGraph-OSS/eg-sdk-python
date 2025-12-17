# ValidationsApiDbEnvironmentsV1TestConnectionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**can_connect** | **bool** |  | [optional] 
**reason_failed** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_db_environments_v1_test_connection_response import ValidationsApiDbEnvironmentsV1TestConnectionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiDbEnvironmentsV1TestConnectionResponse from a JSON string
validations_api_db_environments_v1_test_connection_response_instance = ValidationsApiDbEnvironmentsV1TestConnectionResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiDbEnvironmentsV1TestConnectionResponse.to_json())

# convert the object into a dict
validations_api_db_environments_v1_test_connection_response_dict = validations_api_db_environments_v1_test_connection_response_instance.to_dict()
# create an instance of ValidationsApiDbEnvironmentsV1TestConnectionResponse from a dict
validations_api_db_environments_v1_test_connection_response_from_dict = ValidationsApiDbEnvironmentsV1TestConnectionResponse.from_dict(validations_api_db_environments_v1_test_connection_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


