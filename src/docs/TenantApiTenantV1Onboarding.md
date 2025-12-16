# TenantApiTenantV1Onboarding


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | [optional] 
**progress_percentage** | **float** |  | [optional] 
**total_steps** | **int** |  | [optional] 
**last_completed_step** | **int** |  | [optional] 
**started_at** | **str** |  | [optional] 
**completed_at** | **str** |  | [optional] 
**steps** | [**List[TenantApiTenantV1OnboardingStep]**](TenantApiTenantV1OnboardingStep.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_onboarding import TenantApiTenantV1Onboarding

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1Onboarding from a JSON string
tenant_api_tenant_v1_onboarding_instance = TenantApiTenantV1Onboarding.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1Onboarding.to_json())

# convert the object into a dict
tenant_api_tenant_v1_onboarding_dict = tenant_api_tenant_v1_onboarding_instance.to_dict()
# create an instance of TenantApiTenantV1Onboarding from a dict
tenant_api_tenant_v1_onboarding_from_dict = TenantApiTenantV1Onboarding.from_dict(tenant_api_tenant_v1_onboarding_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


