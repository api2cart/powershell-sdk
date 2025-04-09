# Image
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**HttpPath** | **String** |  | [optional] 
**FileName** | **String** |  | [optional] 
**MimeType** | **String** |  | [optional] 
**Size** | **Int32** |  | [optional] 
**CreateAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ModifiedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Alt** | **String** |  | [optional] 
**Avail** | **Boolean** |  | [optional] 
**SortOrder** | **Int32** |  | [optional] 
**Type** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Image = Initialize-PSOpenAPIToolsImage  -Id null `
 -HttpPath null `
 -FileName null `
 -MimeType null `
 -Size null `
 -CreateAt null `
 -ModifiedAt null `
 -Alt null `
 -Avail null `
 -SortOrder null `
 -Type null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Image | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

