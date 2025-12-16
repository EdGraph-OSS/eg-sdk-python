# TenantApiTenantV1TenantProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**tenant_types** | [**List[TenantApiTenantV1TenantType]**](TenantApiTenantV1TenantType.md) |  | [optional] [readonly] 
**organization_identifier** | **str** |  | [optional] 
**organization_name** | **str** |  | [optional] 
**state** | **str** |  | [optional] 
**tenant_status** | [**TenantApiTenantV1TenantStatus**](TenantApiTenantV1TenantStatus.md) |  | [optional] 
**is_demo** | **bool** |  | [optional] 
**subscriptions_migrated** | **bool** |  | [optional] 
**subscriptions** | [**List[TenantApiTenantV1SubscriptionProfileResponse]**](TenantApiTenantV1SubscriptionProfileResponse.md) |  | [optional] [readonly] 
**domains** | [**List[TenantApiTenantV1DomainProfileResponse]**](TenantApiTenantV1DomainProfileResponse.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**identity_providers** | [**List[TenantApiTenantV1TenantIdentityProviders]**](TenantApiTenantV1TenantIdentityProviders.md) |  | [optional] [readonly] 
**onboarding** | [**TenantApiTenantV1Onboarding**](TenantApiTenantV1Onboarding.md) |  | [optional] 
**organizations** | [**List[TenantApiTenantV1Organization]**](TenantApiTenantV1Organization.md) |  | [optional] [readonly] 
**organization_identifier_hash** | **str** |  | [optional] 
**settings** | [**List[TenantApiTenantV1TenantSetting]**](TenantApiTenantV1TenantSetting.md) |  | [optional] [readonly] 
**additional_settings** | [**TenantApiTenantV1TenantAdditionalSetting**](TenantApiTenantV1TenantAdditionalSetting.md) |  | [optional] 
**tenant_type** | **str** |  | [optional] 
**security_score** | **float** |  | [optional] 
**organizational_account_rating** | **float** |  | [optional] 
**multi_factor_authentication_rating** | **float** |  | [optional] 
**domain_verification_rating** | **float** |  | [optional] 
**deployment_type** | [**TenantApiTenantV1DeploymentType**](TenantApiTenantV1DeploymentType.md) |  | [optional] 
**branding** | [**TenantApiTenantV1TenantBrandingResponse**](TenantApiTenantV1TenantBrandingResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_tenant_profile_response import TenantApiTenantV1TenantProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1TenantProfileResponse from a JSON string
tenant_api_tenant_v1_tenant_profile_response_instance = TenantApiTenantV1TenantProfileResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1TenantProfileResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_tenant_profile_response_dict = tenant_api_tenant_v1_tenant_profile_response_instance.to_dict()
# create an instance of TenantApiTenantV1TenantProfileResponse from a dict
tenant_api_tenant_v1_tenant_profile_response_from_dict = TenantApiTenantV1TenantProfileResponse.from_dict(tenant_api_tenant_v1_tenant_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


