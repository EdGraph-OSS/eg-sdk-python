# ValidationsApiDbEnvironmentsV1CreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** | Details | [optional] 
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**connection_type** | **str** | Connection | [optional] 
**sql_server_connection** | [**ValidationsApiDbEnvironmentsV1SqlServerConnection**](ValidationsApiDbEnvironmentsV1SqlServerConnection.md) |  | [optional] 
**azure_synapse_sql_serverless_connection** | [**ValidationsApiDbEnvironmentsV1AzureSynapseSqlServerlessConnection**](ValidationsApiDbEnvironmentsV1AzureSynapseSqlServerlessConnection.md) |  | [optional] 
**max_number_results** | **int** | Metadata | [optional] 
**timeout_in_minutes** | **int** |  | [optional] 
**version** | **int** |  | [optional] 
**map_tables** | **str** |  | [optional] 
**instance_type** | [**ValidationsApiCoreV1InstanceType**](ValidationsApiCoreV1InstanceType.md) |  | [optional] 
**provider** | [**ValidationsApiCoreV1Provider**](ValidationsApiCoreV1Provider.md) |  | [optional] 
**is_default** | **bool** |  | [optional] 
**metadata_json** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_db_environments_v1_create_request import ValidationsApiDbEnvironmentsV1CreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiDbEnvironmentsV1CreateRequest from a JSON string
validations_api_db_environments_v1_create_request_instance = ValidationsApiDbEnvironmentsV1CreateRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiDbEnvironmentsV1CreateRequest.to_json())

# convert the object into a dict
validations_api_db_environments_v1_create_request_dict = validations_api_db_environments_v1_create_request_instance.to_dict()
# create an instance of ValidationsApiDbEnvironmentsV1CreateRequest from a dict
validations_api_db_environments_v1_create_request_from_dict = ValidationsApiDbEnvironmentsV1CreateRequest.from_dict(validations_api_db_environments_v1_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


