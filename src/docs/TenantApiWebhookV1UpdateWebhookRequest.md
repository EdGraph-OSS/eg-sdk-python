# TenantApiWebhookV1UpdateWebhookRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**secret_header** | **str** |  | [optional] 
**secret_value** | **str** |  | [optional] 
**content_type** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**event_subscriptions** | [**List[TenantApiWebhookV1WebhookSubscriberResponse]**](TenantApiWebhookV1WebhookSubscriberResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.tenant_api_webhook_v1_update_webhook_request import TenantApiWebhookV1UpdateWebhookRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiWebhookV1UpdateWebhookRequest from a JSON string
tenant_api_webhook_v1_update_webhook_request_instance = TenantApiWebhookV1UpdateWebhookRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiWebhookV1UpdateWebhookRequest.to_json())

# convert the object into a dict
tenant_api_webhook_v1_update_webhook_request_dict = tenant_api_webhook_v1_update_webhook_request_instance.to_dict()
# create an instance of TenantApiWebhookV1UpdateWebhookRequest from a dict
tenant_api_webhook_v1_update_webhook_request_from_dict = TenantApiWebhookV1UpdateWebhookRequest.from_dict(tenant_api_webhook_v1_update_webhook_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


