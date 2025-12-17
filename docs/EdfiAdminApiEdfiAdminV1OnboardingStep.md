# EdfiAdminApiEdfiAdminV1OnboardingStep


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**number** | **int** |  | [optional] 
**description** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**started_at** | **str** |  | [optional] 
**completed_at** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_onboarding_step import EdfiAdminApiEdfiAdminV1OnboardingStep

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1OnboardingStep from a JSON string
edfi_admin_api_edfi_admin_v1_onboarding_step_instance = EdfiAdminApiEdfiAdminV1OnboardingStep.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1OnboardingStep.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_onboarding_step_dict = edfi_admin_api_edfi_admin_v1_onboarding_step_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1OnboardingStep from a dict
edfi_admin_api_edfi_admin_v1_onboarding_step_from_dict = EdfiAdminApiEdfiAdminV1OnboardingStep.from_dict(edfi_admin_api_edfi_admin_v1_onboarding_step_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


