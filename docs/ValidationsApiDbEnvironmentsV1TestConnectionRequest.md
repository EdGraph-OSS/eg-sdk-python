# ValidationsApiDbEnvironmentsV1TestConnectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**connection_type** | **str** |  | [optional] 
**sql_server_connection** | [**ValidationsApiDbEnvironmentsV1SqlServerConnection**](ValidationsApiDbEnvironmentsV1SqlServerConnection.md) |  | [optional] 
**azure_synapse_sql_serverless_connection** | [**ValidationsApiDbEnvironmentsV1AzureSynapseSqlServerlessConnection**](ValidationsApiDbEnvironmentsV1AzureSynapseSqlServerlessConnection.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_db_environments_v1_test_connection_request import ValidationsApiDbEnvironmentsV1TestConnectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiDbEnvironmentsV1TestConnectionRequest from a JSON string
validations_api_db_environments_v1_test_connection_request_instance = ValidationsApiDbEnvironmentsV1TestConnectionRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiDbEnvironmentsV1TestConnectionRequest.to_json())

# convert the object into a dict
validations_api_db_environments_v1_test_connection_request_dict = validations_api_db_environments_v1_test_connection_request_instance.to_dict()
# create an instance of ValidationsApiDbEnvironmentsV1TestConnectionRequest from a dict
validations_api_db_environments_v1_test_connection_request_from_dict = ValidationsApiDbEnvironmentsV1TestConnectionRequest.from_dict(validations_api_db_environments_v1_test_connection_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


