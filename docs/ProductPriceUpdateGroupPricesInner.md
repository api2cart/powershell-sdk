# ProductPriceUpdateGroupPricesInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **Int32** |  | [optional] 
**GroupId** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductPriceUpdateGroupPricesInner = Initialize-PSOpenAPIToolsProductPriceUpdateGroupPricesInner  -Id null `
 -GroupId null `
 -Price null
```

- Convert the resource to JSON
```powershell
$ProductPriceUpdateGroupPricesInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

