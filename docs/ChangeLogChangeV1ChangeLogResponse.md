# ChangeLogChangeV1ChangeLogResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**source** | **str** |  | [optional] 
**trace_id** | **str** |  | [optional] 
**correlation_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**produced_by** | **str** |  | [optional] 
**produced_date_time** | **str** |  | [optional] 
**producer_client_id** | **str** |  | [optional] 
**producer_address** | **str** |  | [optional] 
**entity_type** | **str** |  | [optional] 
**entity_id** | **str** |  | [optional] 
**event_type** | **str** |  | [optional] 
**event_id** | **str** |  | [optional] 
**event_payload** | [**GoogleProtobufWellKnownTypesStruct**](GoogleProtobufWellKnownTypesStruct.md) |  | [optional] 
**event_schema** | [**GoogleProtobufWellKnownTypesStruct**](GoogleProtobufWellKnownTypesStruct.md) |  | [optional] 
**event_version** | **str** |  | [optional] 
**extensions** | [**GoogleProtobufWellKnownTypesStruct**](GoogleProtobufWellKnownTypesStruct.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.change_log_change_v1_change_log_response import ChangeLogChangeV1ChangeLogResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ChangeLogChangeV1ChangeLogResponse from a JSON string
change_log_change_v1_change_log_response_instance = ChangeLogChangeV1ChangeLogResponse.from_json(json)
# print the JSON string representation of the object
print(ChangeLogChangeV1ChangeLogResponse.to_json())

# convert the object into a dict
change_log_change_v1_change_log_response_dict = change_log_change_v1_change_log_response_instance.to_dict()
# create an instance of ChangeLogChangeV1ChangeLogResponse from a dict
change_log_change_v1_change_log_response_from_dict = ChangeLogChangeV1ChangeLogResponse.from_dict(change_log_change_v1_change_log_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


