# TenantApiSectionsV1SchoolListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**school_id** | **int** |  | [optional] 
**school_year** | **int** |  | [optional] 
**school_name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_sections_v1_school_list_response import TenantApiSectionsV1SchoolListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiSectionsV1SchoolListResponse from a JSON string
tenant_api_sections_v1_school_list_response_instance = TenantApiSectionsV1SchoolListResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiSectionsV1SchoolListResponse.to_json())

# convert the object into a dict
tenant_api_sections_v1_school_list_response_dict = tenant_api_sections_v1_school_list_response_instance.to_dict()
# create an instance of TenantApiSectionsV1SchoolListResponse from a dict
tenant_api_sections_v1_school_list_response_from_dict = TenantApiSectionsV1SchoolListResponse.from_dict(tenant_api_sections_v1_school_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


