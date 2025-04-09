# ReturnOrderProduct
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **String** |  | [optional] 
**OrderProductId** | **String** |  | [optional] 
**Sku** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Quantity** | **Int32** |  | [optional] 
**Reason** | [**ReturnReason**](ReturnReason.md) |  | [optional] 
**Action** | [**ReturnAction**](ReturnAction.md) |  | [optional] 
**Condition** | **String** |  | [optional] 
**CustomerComment** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ReturnOrderProduct = Initialize-PSOpenAPIToolsReturnOrderProduct  -ProductId null `
 -OrderProductId null `
 -Sku null `
 -Name null `
 -Quantity null `
 -Reason null `
 -Action null `
 -Condition null `
 -CustomerComment null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ReturnOrderProduct | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

