# CartShippingMethod
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **String** |  | [optional] 
**HandlingFee** | **String** |  | [optional] 
**HandlingEnabled** | **String** |  | [optional] 
**HandlingType** | **String** |  | [optional] 
**DefaultPrice** | **String** |  | [optional] 
**DefaultPriceType** | **String** |  | [optional] 
**Type** | **String** |  | [optional] 
**Enabled** | **String** |  | [optional] 
**MinOrderAmount** | **String** |  | [optional] 
**Rates** | [**CartShippingMethodRate[]**](CartShippingMethodRate.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CartShippingMethod = Initialize-PSOpenAPIToolsCartShippingMethod  -Name null `
 -HandlingFee null `
 -HandlingEnabled null `
 -HandlingType null `
 -DefaultPrice null `
 -DefaultPriceType null `
 -Type null `
 -Enabled null `
 -MinOrderAmount null `
 -Rates null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CartShippingMethod | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

