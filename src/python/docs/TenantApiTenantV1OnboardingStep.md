# TenantApiTenantV1OnboardingStep


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**number** | **int** |  | [optional] 
**description** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**started_at** | **str** |  | [optional] 
**completed_at** | **str** |  | [optional] 
**details** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_onboarding_step import TenantApiTenantV1OnboardingStep

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1OnboardingStep from a JSON string
tenant_api_tenant_v1_onboarding_step_instance = TenantApiTenantV1OnboardingStep.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1OnboardingStep.to_json())

# convert the object into a dict
tenant_api_tenant_v1_onboarding_step_dict = tenant_api_tenant_v1_onboarding_step_instance.to_dict()
# create an instance of TenantApiTenantV1OnboardingStep from a dict
tenant_api_tenant_v1_onboarding_step_from_dict = TenantApiTenantV1OnboardingStep.from_dict(tenant_api_tenant_v1_onboarding_step_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


