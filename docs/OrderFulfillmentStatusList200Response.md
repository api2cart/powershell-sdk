# OrderFulfillmentStatusList200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**OrderFulfillmentStatusList200ResponseResult**](OrderFulfillmentStatusList200ResponseResult.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderFulfillmentStatusList200Response = Initialize-PSOpenAPIToolsOrderFulfillmentStatusList200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$OrderFulfillmentStatusList200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

