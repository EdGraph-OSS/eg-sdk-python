# EdfiAdminApiEdfiAdminV1Onboarding


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | [optional] 
**progress_percentage** | **float** |  | [optional] 
**total_steps** | **int** |  | [optional] 
**last_completed_step** | **int** |  | [optional] 
**started_at** | **str** |  | [optional] 
**completed_at** | **str** |  | [optional] 
**steps** | [**List[EdfiAdminApiEdfiAdminV1OnboardingStep]**](EdfiAdminApiEdfiAdminV1OnboardingStep.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_onboarding import EdfiAdminApiEdfiAdminV1Onboarding

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1Onboarding from a JSON string
edfi_admin_api_edfi_admin_v1_onboarding_instance = EdfiAdminApiEdfiAdminV1Onboarding.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1Onboarding.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_onboarding_dict = edfi_admin_api_edfi_admin_v1_onboarding_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1Onboarding from a dict
edfi_admin_api_edfi_admin_v1_onboarding_from_dict = EdfiAdminApiEdfiAdminV1Onboarding.from_dict(edfi_admin_api_edfi_admin_v1_onboarding_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


