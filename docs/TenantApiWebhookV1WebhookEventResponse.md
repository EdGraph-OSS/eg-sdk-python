# TenantApiWebhookV1WebhookEventResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**created_at** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**updated_by** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**provider** | **str** |  | [optional] 
**group** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**scope** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.tenant_api_webhook_v1_webhook_event_response import TenantApiWebhookV1WebhookEventResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiWebhookV1WebhookEventResponse from a JSON string
tenant_api_webhook_v1_webhook_event_response_instance = TenantApiWebhookV1WebhookEventResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiWebhookV1WebhookEventResponse.to_json())

# convert the object into a dict
tenant_api_webhook_v1_webhook_event_response_dict = tenant_api_webhook_v1_webhook_event_response_instance.to_dict()
# create an instance of TenantApiWebhookV1WebhookEventResponse from a dict
tenant_api_webhook_v1_webhook_event_response_from_dict = TenantApiWebhookV1WebhookEventResponse.from_dict(tenant_api_webhook_v1_webhook_event_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


