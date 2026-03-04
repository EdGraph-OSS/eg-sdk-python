# GoogleProtobufWellKnownTypesValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**null_value** | [**GoogleProtobufWellKnownTypesNullValue**](GoogleProtobufWellKnownTypesNullValue.md) |  | [optional] 
**has_null_value** | **bool** |  | [optional] [readonly] 
**number_value** | **float** |  | [optional] 
**has_number_value** | **bool** |  | [optional] [readonly] 
**string_value** | **str** |  | [optional] 
**has_string_value** | **bool** |  | [optional] [readonly] 
**bool_value** | **bool** |  | [optional] 
**has_bool_value** | **bool** |  | [optional] [readonly] 
**struct_value** | [**GoogleProtobufWellKnownTypesStruct**](GoogleProtobufWellKnownTypesStruct.md) |  | [optional] 
**list_value** | [**GoogleProtobufWellKnownTypesListValue**](GoogleProtobufWellKnownTypesListValue.md) |  | [optional] 
**kind_case** | [**GoogleProtobufWellKnownTypesValueKindOneofCase**](GoogleProtobufWellKnownTypesValueKindOneofCase.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.google_protobuf_well_known_types_value import GoogleProtobufWellKnownTypesValue

# TODO update the JSON string below
json = "{}"
# create an instance of GoogleProtobufWellKnownTypesValue from a JSON string
google_protobuf_well_known_types_value_instance = GoogleProtobufWellKnownTypesValue.from_json(json)
# print the JSON string representation of the object
print(GoogleProtobufWellKnownTypesValue.to_json())

# convert the object into a dict
google_protobuf_well_known_types_value_dict = google_protobuf_well_known_types_value_instance.to_dict()
# create an instance of GoogleProtobufWellKnownTypesValue from a dict
google_protobuf_well_known_types_value_from_dict = GoogleProtobufWellKnownTypesValue.from_dict(google_protobuf_well_known_types_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


