# AccountCartList200ResponseResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CartsCount** | **Int32** |  | [optional] 
**Carts** | [**AccountCartList200ResponseResultCartsInner[]**](AccountCartList200ResponseResultCartsInner.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$AccountCartList200ResponseResult = Initialize-PSOpenAPIToolsAccountCartList200ResponseResult  -CartsCount null `
 -Carts null
```

- Convert the resource to JSON
```powershell
$AccountCartList200ResponseResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

