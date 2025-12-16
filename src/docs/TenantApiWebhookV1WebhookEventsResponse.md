# TenantApiWebhookV1WebhookEventsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_subscriptions** | [**List[TenantApiWebhookV1WebhookSubscriberResponse]**](TenantApiWebhookV1WebhookSubscriberResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.tenant_api_webhook_v1_webhook_events_response import TenantApiWebhookV1WebhookEventsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiWebhookV1WebhookEventsResponse from a JSON string
tenant_api_webhook_v1_webhook_events_response_instance = TenantApiWebhookV1WebhookEventsResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiWebhookV1WebhookEventsResponse.to_json())

# convert the object into a dict
tenant_api_webhook_v1_webhook_events_response_dict = tenant_api_webhook_v1_webhook_events_response_instance.to_dict()
# create an instance of TenantApiWebhookV1WebhookEventsResponse from a dict
tenant_api_webhook_v1_webhook_events_response_from_dict = TenantApiWebhookV1WebhookEventsResponse.from_dict(tenant_api_webhook_v1_webhook_events_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


