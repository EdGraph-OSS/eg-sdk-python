# IMSAdminApiV1InstancesPagedInstancesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[IMSAdminApiV1InstancesInstanceListResponse]**](IMSAdminApiV1InstancesInstanceListResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_instances_paged_instances_response import IMSAdminApiV1InstancesPagedInstancesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1InstancesPagedInstancesResponse from a JSON string
ims_admin_api_v1_instances_paged_instances_response_instance = IMSAdminApiV1InstancesPagedInstancesResponse.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1InstancesPagedInstancesResponse.to_json())

# convert the object into a dict
ims_admin_api_v1_instances_paged_instances_response_dict = ims_admin_api_v1_instances_paged_instances_response_instance.to_dict()
# create an instance of IMSAdminApiV1InstancesPagedInstancesResponse from a dict
ims_admin_api_v1_instances_paged_instances_response_from_dict = IMSAdminApiV1InstancesPagedInstancesResponse.from_dict(ims_admin_api_v1_instances_paged_instances_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


