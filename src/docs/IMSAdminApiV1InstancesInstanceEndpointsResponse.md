# IMSAdminApiV1InstancesInstanceEndpointsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**token_url** | **str** |  | [optional] 
**resources_url** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_instances_instance_endpoints_response import IMSAdminApiV1InstancesInstanceEndpointsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1InstancesInstanceEndpointsResponse from a JSON string
ims_admin_api_v1_instances_instance_endpoints_response_instance = IMSAdminApiV1InstancesInstanceEndpointsResponse.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1InstancesInstanceEndpointsResponse.to_json())

# convert the object into a dict
ims_admin_api_v1_instances_instance_endpoints_response_dict = ims_admin_api_v1_instances_instance_endpoints_response_instance.to_dict()
# create an instance of IMSAdminApiV1InstancesInstanceEndpointsResponse from a dict
ims_admin_api_v1_instances_instance_endpoints_response_from_dict = IMSAdminApiV1InstancesInstanceEndpointsResponse.from_dict(ims_admin_api_v1_instances_instance_endpoints_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


