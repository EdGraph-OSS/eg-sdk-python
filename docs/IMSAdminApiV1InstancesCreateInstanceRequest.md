# IMSAdminApiV1InstancesCreateInstanceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**use_custom_id** | **bool** |  | [optional] 
**custom_id** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**connection_id** | **str** |  | [optional] 
**tier** | **str** |  | [optional] 
**backup_code** | **str** |  | [optional] 
**school_year** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_instances_create_instance_request import IMSAdminApiV1InstancesCreateInstanceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1InstancesCreateInstanceRequest from a JSON string
ims_admin_api_v1_instances_create_instance_request_instance = IMSAdminApiV1InstancesCreateInstanceRequest.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1InstancesCreateInstanceRequest.to_json())

# convert the object into a dict
ims_admin_api_v1_instances_create_instance_request_dict = ims_admin_api_v1_instances_create_instance_request_instance.to_dict()
# create an instance of IMSAdminApiV1InstancesCreateInstanceRequest from a dict
ims_admin_api_v1_instances_create_instance_request_from_dict = IMSAdminApiV1InstancesCreateInstanceRequest.from_dict(ims_admin_api_v1_instances_create_instance_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


