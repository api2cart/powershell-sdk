# Currency
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Iso3** | **String** |  | [optional] 
**SymbolLeft** | **String** |  | [optional] 
**SymbolRight** | **String** |  | [optional] 
**Rate** | **Decimal** |  | [optional] 
**Avail** | **Boolean** |  | [optional] 
**Default** | **Boolean** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Currency = Initialize-PSOpenAPIToolsCurrency  -Id null `
 -Name null `
 -Iso3 null `
 -SymbolLeft null `
 -SymbolRight null `
 -Rate null `
 -Avail null `
 -Default null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Currency | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

