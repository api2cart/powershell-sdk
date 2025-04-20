# ProductAddLogisticInfoInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LogisticId** | **Decimal** |  | 
**IsFree** | **Boolean** |  | [optional] 
**ShippingFee** | **Decimal** |  | [optional] 
**SizeId** | **Decimal** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddLogisticInfoInner = Initialize-PSOpenAPIToolsProductAddLogisticInfoInner  -LogisticId null `
 -IsFree null `
 -ShippingFee null `
 -SizeId null
```

- Convert the resource to JSON
```powershell
$ProductAddLogisticInfoInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

