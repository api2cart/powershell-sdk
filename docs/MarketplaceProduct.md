# MarketplaceProduct
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Type** | **String** |  | [optional] 
**UAsin** | **String** |  | [optional] 
**UEan** | **String** |  | [optional] 
**UGtin** | **String** |  | [optional] 
**UIsbn** | **String** |  | [optional] 
**UMpn** | **String** |  | [optional] 
**UUpc** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**Url** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**Images** | [**Image[]**](Image.md) |  | [optional] 
**ProductOptions** | [**ProductOption[]**](ProductOption.md) |  | [optional] 
**Manufacturer** | **String** |  | [optional] 
**Brand** | **String** |  | [optional] 
**Weight** | **Decimal** |  | [optional] 
**WeightUnit** | **String** |  | [optional] 
**DimensionsUnit** | **String** |  | [optional] 
**Width** | **Decimal** |  | [optional] 
**Height** | **Decimal** |  | [optional] 
**Length** | **Decimal** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$MarketplaceProduct = Initialize-PSOpenAPIToolsMarketplaceProduct  -Id null `
 -Type null `
 -UAsin null `
 -UEan null `
 -UGtin null `
 -UIsbn null `
 -UMpn null `
 -UUpc null `
 -Name null `
 -Description null `
 -Url null `
 -Price null `
 -Images null `
 -ProductOptions null `
 -Manufacturer null `
 -Brand null `
 -Weight null `
 -WeightUnit null `
 -DimensionsUnit null `
 -Width null `
 -Height null `
 -Length null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$MarketplaceProduct | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

