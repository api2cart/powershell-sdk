# CustomerAddress
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Type** | **String** |  | [optional] 
**FirstName** | **String** |  | [optional] 
**LastName** | **String** |  | [optional] 
**Postcode** | **String** |  | [optional] 
**Address1** | **String** |  | [optional] 
**Address2** | **String** |  | [optional] 
**Phone** | **String** |  | [optional] 
**PhoneMobile** | **String** |  | [optional] 
**City** | **String** |  | [optional] 
**Country** | [**Country**](Country.md) |  | [optional] 
**State** | [**State**](State.md) |  | [optional] 
**Company** | **String** |  | [optional] 
**Fax** | **String** |  | [optional] 
**Website** | **String** |  | [optional] 
**Gender** | **String** |  | [optional] 
**Region** | **String** |  | [optional] 
**Default** | **Boolean** |  | [optional] 
**TaxId** | **String** |  | [optional] 
**IdentificationNumber** | **String** |  | [optional] 
**Alias** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CustomerAddress = Initialize-PSOpenAPIToolsCustomerAddress  -Id null `
 -Type null `
 -FirstName null `
 -LastName null `
 -Postcode null `
 -Address1 null `
 -Address2 null `
 -Phone null `
 -PhoneMobile null `
 -City null `
 -Country null `
 -State null `
 -Company null `
 -Fax null `
 -Website null `
 -Gender null `
 -Region null `
 -Default null `
 -TaxId null `
 -IdentificationNumber null `
 -Alias null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CustomerAddress | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

