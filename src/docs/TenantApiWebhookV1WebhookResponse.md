# TenantApiWebhookV1WebhookResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**created_at** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**updated_by** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**name** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**secret_header** | **str** |  | [optional] 
**secret_value** | **str** |  | [optional] 
**content_type** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**event_subscriptions** | [**List[TenantApiWebhookV1WebhookSubscriberResponse]**](TenantApiWebhookV1WebhookSubscriberResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.tenant_api_webhook_v1_webhook_response import TenantApiWebhookV1WebhookResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiWebhookV1WebhookResponse from a JSON string
tenant_api_webhook_v1_webhook_response_instance = TenantApiWebhookV1WebhookResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiWebhookV1WebhookResponse.to_json())

# convert the object into a dict
tenant_api_webhook_v1_webhook_response_dict = tenant_api_webhook_v1_webhook_response_instance.to_dict()
# create an instance of TenantApiWebhookV1WebhookResponse from a dict
tenant_api_webhook_v1_webhook_response_from_dict = TenantApiWebhookV1WebhookResponse.from_dict(tenant_api_webhook_v1_webhook_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


