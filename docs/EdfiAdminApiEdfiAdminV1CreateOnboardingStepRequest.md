# EdfiAdminApiEdfiAdminV1CreateOnboardingStepRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instance_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**number** | **int** |  | [optional] 
**description** | **str** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_onboarding_step_request import EdfiAdminApiEdfiAdminV1CreateOnboardingStepRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1CreateOnboardingStepRequest from a JSON string
edfi_admin_api_edfi_admin_v1_create_onboarding_step_request_instance = EdfiAdminApiEdfiAdminV1CreateOnboardingStepRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1CreateOnboardingStepRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_create_onboarding_step_request_dict = edfi_admin_api_edfi_admin_v1_create_onboarding_step_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1CreateOnboardingStepRequest from a dict
edfi_admin_api_edfi_admin_v1_create_onboarding_step_request_from_dict = EdfiAdminApiEdfiAdminV1CreateOnboardingStepRequest.from_dict(edfi_admin_api_edfi_admin_v1_create_onboarding_step_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


