# ValidationsApiDbEnvironmentsV1SqlServerConnection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**server** | **str** |  | [optional] 
**database** | **str** |  | [optional] 
**username** | **str** |  | [optional] 
**password** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_db_environments_v1_sql_server_connection import ValidationsApiDbEnvironmentsV1SqlServerConnection

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiDbEnvironmentsV1SqlServerConnection from a JSON string
validations_api_db_environments_v1_sql_server_connection_instance = ValidationsApiDbEnvironmentsV1SqlServerConnection.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiDbEnvironmentsV1SqlServerConnection.to_json())

# convert the object into a dict
validations_api_db_environments_v1_sql_server_connection_dict = validations_api_db_environments_v1_sql_server_connection_instance.to_dict()
# create an instance of ValidationsApiDbEnvironmentsV1SqlServerConnection from a dict
validations_api_db_environments_v1_sql_server_connection_from_dict = ValidationsApiDbEnvironmentsV1SqlServerConnection.from_dict(validations_api_db_environments_v1_sql_server_connection_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


