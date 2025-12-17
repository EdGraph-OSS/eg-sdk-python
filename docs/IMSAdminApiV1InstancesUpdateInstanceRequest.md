# IMSAdminApiV1InstancesUpdateInstanceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instance_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_instances_update_instance_request import IMSAdminApiV1InstancesUpdateInstanceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1InstancesUpdateInstanceRequest from a JSON string
ims_admin_api_v1_instances_update_instance_request_instance = IMSAdminApiV1InstancesUpdateInstanceRequest.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1InstancesUpdateInstanceRequest.to_json())

# convert the object into a dict
ims_admin_api_v1_instances_update_instance_request_dict = ims_admin_api_v1_instances_update_instance_request_instance.to_dict()
# create an instance of IMSAdminApiV1InstancesUpdateInstanceRequest from a dict
ims_admin_api_v1_instances_update_instance_request_from_dict = IMSAdminApiV1InstancesUpdateInstanceRequest.from_dict(ims_admin_api_v1_instances_update_instance_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


