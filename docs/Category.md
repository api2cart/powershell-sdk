# Category
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**ParentId** | **String** |  | [optional] 
**CreatedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ModifiedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Name** | **String** |  | [optional] 
**ShortDescription** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**StoresIds** | **String[]** |  | [optional] 
**Keywords** | **String** |  | [optional] 
**MetaDescription** | **String** |  | [optional] 
**MetaTitle** | **String** |  | [optional] 
**Avail** | **Boolean** |  | [optional] 
**Path** | **String** |  | [optional] 
**SeoUrl** | **String** |  | [optional] 
**SortOrder** | **Int32** |  | [optional] 
**Images** | [**Image[]**](Image.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Category = Initialize-PSOpenAPIToolsCategory  -Id null `
 -ParentId null `
 -CreatedAt null `
 -ModifiedAt null `
 -Name null `
 -ShortDescription null `
 -Description null `
 -StoresIds null `
 -Keywords null `
 -MetaDescription null `
 -MetaTitle null `
 -Avail null `
 -Path null `
 -SeoUrl null `
 -SortOrder null `
 -Images null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Category | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

