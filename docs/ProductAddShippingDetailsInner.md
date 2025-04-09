# ProductAddShippingDetailsInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ShippingType** | **String** |  | [optional] 
**ShippingService** | **String** |  | [optional] 
**ShippingCost** | **Decimal** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddShippingDetailsInner = Initialize-PSOpenAPIToolsProductAddShippingDetailsInner  -ShippingType null `
 -ShippingService null `
 -ShippingCost null
```

- Convert the resource to JSON
```powershell
$ProductAddShippingDetailsInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

