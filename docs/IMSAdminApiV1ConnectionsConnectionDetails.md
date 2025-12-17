# IMSAdminApiV1ConnectionsConnectionDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**metadata** | [**List[IMSAdminApiV1ConnectionsConnectionDetailsMetadata]**](IMSAdminApiV1ConnectionsConnectionDetailsMetadata.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_connections_connection_details import IMSAdminApiV1ConnectionsConnectionDetails

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1ConnectionsConnectionDetails from a JSON string
ims_admin_api_v1_connections_connection_details_instance = IMSAdminApiV1ConnectionsConnectionDetails.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1ConnectionsConnectionDetails.to_json())

# convert the object into a dict
ims_admin_api_v1_connections_connection_details_dict = ims_admin_api_v1_connections_connection_details_instance.to_dict()
# create an instance of IMSAdminApiV1ConnectionsConnectionDetails from a dict
ims_admin_api_v1_connections_connection_details_from_dict = IMSAdminApiV1ConnectionsConnectionDetails.from_dict(ims_admin_api_v1_connections_connection_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


