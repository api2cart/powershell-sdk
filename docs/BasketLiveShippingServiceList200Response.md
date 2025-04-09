# BasketLiveShippingServiceList200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**BasketLiveShippingServiceList200ResponseResult**](BasketLiveShippingServiceList200ResponseResult.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$BasketLiveShippingServiceList200Response = Initialize-PSOpenAPIToolsBasketLiveShippingServiceList200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$BasketLiveShippingServiceList200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

