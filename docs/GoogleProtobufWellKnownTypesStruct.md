# GoogleProtobufWellKnownTypesStruct


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**fields** | [**Dict[str, GoogleProtobufWellKnownTypesValue]**](GoogleProtobufWellKnownTypesValue.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.google_protobuf_well_known_types_struct import GoogleProtobufWellKnownTypesStruct

# TODO update the JSON string below
json = "{}"
# create an instance of GoogleProtobufWellKnownTypesStruct from a JSON string
google_protobuf_well_known_types_struct_instance = GoogleProtobufWellKnownTypesStruct.from_json(json)
# print the JSON string representation of the object
print(GoogleProtobufWellKnownTypesStruct.to_json())

# convert the object into a dict
google_protobuf_well_known_types_struct_dict = google_protobuf_well_known_types_struct_instance.to_dict()
# create an instance of GoogleProtobufWellKnownTypesStruct from a dict
google_protobuf_well_known_types_struct_from_dict = GoogleProtobufWellKnownTypesStruct.from_dict(google_protobuf_well_known_types_struct_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


