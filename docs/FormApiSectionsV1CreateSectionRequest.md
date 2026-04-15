# FormApiSectionsV1CreateSectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**form_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**order** | **int** |  | [optional] 
**sub_heading** | **str** |  | [optional] 
**custom_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_sections_v1_create_section_request import FormApiSectionsV1CreateSectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiSectionsV1CreateSectionRequest from a JSON string
form_api_sections_v1_create_section_request_instance = FormApiSectionsV1CreateSectionRequest.from_json(json)
# print the JSON string representation of the object
print(FormApiSectionsV1CreateSectionRequest.to_json())

# convert the object into a dict
form_api_sections_v1_create_section_request_dict = form_api_sections_v1_create_section_request_instance.to_dict()
# create an instance of FormApiSectionsV1CreateSectionRequest from a dict
form_api_sections_v1_create_section_request_from_dict = FormApiSectionsV1CreateSectionRequest.from_dict(form_api_sections_v1_create_section_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


