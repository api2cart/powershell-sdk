# StoreAttribute
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Code** | **String** |  | [optional] 
**Type** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**DefaultValues** | **String[]** |  | [optional] 
**Position** | **Int32** |  | [optional] 
**Visible** | **Boolean** |  | [optional] 
**Required** | **Boolean** |  | [optional] 
**System** | **Boolean** |  | [optional] 
**Values** | **String[]** |  | [optional] 
**StoreId** | **String** |  | [optional] 
**LangId** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$StoreAttribute = Initialize-PSOpenAPIToolsStoreAttribute  -Id null `
 -Code null `
 -Type null `
 -Name null `
 -DefaultValues null `
 -Position null `
 -Visible null `
 -Required null `
 -System null `
 -Values null `
 -StoreId null `
 -LangId null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$StoreAttribute | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

