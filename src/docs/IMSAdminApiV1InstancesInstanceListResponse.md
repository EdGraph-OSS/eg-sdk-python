# IMSAdminApiV1InstancesInstanceListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instance_id** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**use_custom_id** | **bool** |  | [optional] 
**custom_id** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**connection** | [**IMSAdminApiV1ConnectionsConnectionListResponse**](IMSAdminApiV1ConnectionsConnectionListResponse.md) |  | [optional] 
**tier** | [**IMSAdminApiV1TiersTier**](IMSAdminApiV1TiersTier.md) |  | [optional] 
**backup_code** | [**IMSAdminApiV1DbBackupCodesDbBackupCode**](IMSAdminApiV1DbBackupCodesDbBackupCode.md) |  | [optional] 
**status** | **str** |  | [optional] 
**school_year** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_instances_instance_list_response import IMSAdminApiV1InstancesInstanceListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1InstancesInstanceListResponse from a JSON string
ims_admin_api_v1_instances_instance_list_response_instance = IMSAdminApiV1InstancesInstanceListResponse.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1InstancesInstanceListResponse.to_json())

# convert the object into a dict
ims_admin_api_v1_instances_instance_list_response_dict = ims_admin_api_v1_instances_instance_list_response_instance.to_dict()
# create an instance of IMSAdminApiV1InstancesInstanceListResponse from a dict
ims_admin_api_v1_instances_instance_list_response_from_dict = IMSAdminApiV1InstancesInstanceListResponse.from_dict(ims_admin_api_v1_instances_instance_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


