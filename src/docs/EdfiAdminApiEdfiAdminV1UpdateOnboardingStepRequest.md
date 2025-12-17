# EdfiAdminApiEdfiAdminV1UpdateOnboardingStepRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instance_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**number** | **int** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_onboarding_step_request import EdfiAdminApiEdfiAdminV1UpdateOnboardingStepRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1UpdateOnboardingStepRequest from a JSON string
edfi_admin_api_edfi_admin_v1_update_onboarding_step_request_instance = EdfiAdminApiEdfiAdminV1UpdateOnboardingStepRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1UpdateOnboardingStepRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_update_onboarding_step_request_dict = edfi_admin_api_edfi_admin_v1_update_onboarding_step_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1UpdateOnboardingStepRequest from a dict
edfi_admin_api_edfi_admin_v1_update_onboarding_step_request_from_dict = EdfiAdminApiEdfiAdminV1UpdateOnboardingStepRequest.from_dict(edfi_admin_api_edfi_admin_v1_update_onboarding_step_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


