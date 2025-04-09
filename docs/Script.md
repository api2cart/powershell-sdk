# Script
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**Src** | **String** |  | [optional] 
**Scope** | **String** |  | [optional] 
**VarEvent** | **String** |  | [optional] 
**LoadMethod** | **String** |  | [optional] 
**Html** | **String** |  | [optional] 
**CreatedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ModifiedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Script = Initialize-PSOpenAPIToolsScript  -Id null `
 -Name null `
 -Description null `
 -Src null `
 -Scope null `
 -VarEvent null `
 -LoadMethod null `
 -Html null `
 -CreatedTime null `
 -ModifiedTime null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Script | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

