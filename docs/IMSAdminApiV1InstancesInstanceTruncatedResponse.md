# IMSAdminApiV1InstancesInstanceTruncatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instance_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**details** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_instances_instance_truncated_response import IMSAdminApiV1InstancesInstanceTruncatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1InstancesInstanceTruncatedResponse from a JSON string
ims_admin_api_v1_instances_instance_truncated_response_instance = IMSAdminApiV1InstancesInstanceTruncatedResponse.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1InstancesInstanceTruncatedResponse.to_json())

# convert the object into a dict
ims_admin_api_v1_instances_instance_truncated_response_dict = ims_admin_api_v1_instances_instance_truncated_response_instance.to_dict()
# create an instance of IMSAdminApiV1InstancesInstanceTruncatedResponse from a dict
ims_admin_api_v1_instances_instance_truncated_response_from_dict = IMSAdminApiV1InstancesInstanceTruncatedResponse.from_dict(ims_admin_api_v1_instances_instance_truncated_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


