# IMSAdminApiV1InstancesInstanceCsvExportedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instance_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**status** | [**IMSAdminApiV1InstancesExportState**](IMSAdminApiV1InstancesExportState.md) |  | [optional] 
**details** | **str** |  | [optional] 
**zipped_contents** | **List[int]** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_instances_instance_csv_exported_response import IMSAdminApiV1InstancesInstanceCsvExportedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1InstancesInstanceCsvExportedResponse from a JSON string
ims_admin_api_v1_instances_instance_csv_exported_response_instance = IMSAdminApiV1InstancesInstanceCsvExportedResponse.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1InstancesInstanceCsvExportedResponse.to_json())

# convert the object into a dict
ims_admin_api_v1_instances_instance_csv_exported_response_dict = ims_admin_api_v1_instances_instance_csv_exported_response_instance.to_dict()
# create an instance of IMSAdminApiV1InstancesInstanceCsvExportedResponse from a dict
ims_admin_api_v1_instances_instance_csv_exported_response_from_dict = IMSAdminApiV1InstancesInstanceCsvExportedResponse.from_dict(ims_admin_api_v1_instances_instance_csv_exported_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


