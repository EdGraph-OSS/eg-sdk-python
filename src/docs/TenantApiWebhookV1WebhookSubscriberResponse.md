# TenantApiWebhookV1WebhookSubscriberResponse

Webhook Subscribers

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_name** | **str** |  | [optional] 
**event_version** | **str** |  | [optional] 
**event_schema** | **str** |  | [optional] 
**group_name** | **str** |  | [optional] 
**scope** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.tenant_api_webhook_v1_webhook_subscriber_response import TenantApiWebhookV1WebhookSubscriberResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiWebhookV1WebhookSubscriberResponse from a JSON string
tenant_api_webhook_v1_webhook_subscriber_response_instance = TenantApiWebhookV1WebhookSubscriberResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiWebhookV1WebhookSubscriberResponse.to_json())

# convert the object into a dict
tenant_api_webhook_v1_webhook_subscriber_response_dict = tenant_api_webhook_v1_webhook_subscriber_response_instance.to_dict()
# create an instance of TenantApiWebhookV1WebhookSubscriberResponse from a dict
tenant_api_webhook_v1_webhook_subscriber_response_from_dict = TenantApiWebhookV1WebhookSubscriberResponse.from_dict(tenant_api_webhook_v1_webhook_subscriber_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


