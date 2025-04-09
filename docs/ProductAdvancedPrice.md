# ProductAdvancedPrice
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Value** | **Decimal** |  | [optional] 
**Avail** | **Boolean** |  | [optional] 
**GroupId** | **String** |  | [optional] 
**QuantityFrom** | **Decimal** |  | [optional] 
**StartTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ExpireTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAdvancedPrice = Initialize-PSOpenAPIToolsProductAdvancedPrice  -Id null `
 -Value null `
 -Avail null `
 -GroupId null `
 -QuantityFrom null `
 -StartTime null `
 -ExpireTime null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ProductAdvancedPrice | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

