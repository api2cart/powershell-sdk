# AccountFailedWebhooks200ResponseResultWebhookInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**WebhookId** | **Int32** |  | [optional] 
**EntityId** | **String** |  | [optional] 
**Time** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$AccountFailedWebhooks200ResponseResultWebhookInner = Initialize-PSOpenAPIToolsAccountFailedWebhooks200ResponseResultWebhookInner  -WebhookId null `
 -EntityId null `
 -Time null
```

- Convert the resource to JSON
```powershell
$AccountFailedWebhooks200ResponseResultWebhookInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

