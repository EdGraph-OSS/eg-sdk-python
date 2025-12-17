# IdentityApiUserV1SEOAAResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**seoaa_id** | **str** |  | [optional] 
**education_organization_id** | **int** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**short_name_of_institution** | **str** |  | [optional] 
**staff_classification_descriptor** | **str** |  | [optional] 
**staff_unique_id** | **str** |  | [optional] 
**begin_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 
**source** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_seoaa_response import IdentityApiUserV1SEOAAResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1SEOAAResponse from a JSON string
identity_api_user_v1_seoaa_response_instance = IdentityApiUserV1SEOAAResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1SEOAAResponse.to_json())

# convert the object into a dict
identity_api_user_v1_seoaa_response_dict = identity_api_user_v1_seoaa_response_instance.to_dict()
# create an instance of IdentityApiUserV1SEOAAResponse from a dict
identity_api_user_v1_seoaa_response_from_dict = IdentityApiUserV1SEOAAResponse.from_dict(identity_api_user_v1_seoaa_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


