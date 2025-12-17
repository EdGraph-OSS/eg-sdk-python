# ValidationsApiDbEnvironmentsV1DbEnvironmentDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** | Details | [optional] 
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**connection_type** | **str** | Connection | [optional] 
**sql_server_connection** | [**ValidationsApiDbEnvironmentsV1SqlServerConnection**](ValidationsApiDbEnvironmentsV1SqlServerConnection.md) |  | [optional] 
**azure_synapse_sql_serverless_connection** | [**ValidationsApiDbEnvironmentsV1AzureSynapseSqlServerlessConnection**](ValidationsApiDbEnvironmentsV1AzureSynapseSqlServerlessConnection.md) |  | [optional] 
**connection_string** | **str** |  | [optional] 
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
from edgraph_platform_client.models.validations_api_db_environments_v1_db_environment_dto import ValidationsApiDbEnvironmentsV1DbEnvironmentDto

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiDbEnvironmentsV1DbEnvironmentDto from a JSON string
validations_api_db_environments_v1_db_environment_dto_instance = ValidationsApiDbEnvironmentsV1DbEnvironmentDto.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiDbEnvironmentsV1DbEnvironmentDto.to_json())

# convert the object into a dict
validations_api_db_environments_v1_db_environment_dto_dict = validations_api_db_environments_v1_db_environment_dto_instance.to_dict()
# create an instance of ValidationsApiDbEnvironmentsV1DbEnvironmentDto from a dict
validations_api_db_environments_v1_db_environment_dto_from_dict = ValidationsApiDbEnvironmentsV1DbEnvironmentDto.from_dict(validations_api_db_environments_v1_db_environment_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


