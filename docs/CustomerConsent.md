# CustomerConsent
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Type** | **String** |  | [optional] 
**Status** | **String** |  | [optional] 
**Source** | **String** |  | [optional] 
**OptInLevel** | **String** |  | [optional] 
**ModifiedTime** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CustomerConsent = Initialize-PSOpenAPIToolsCustomerConsent  -Id null `
 -Type null `
 -Status null `
 -Source null `
 -OptInLevel null `
 -ModifiedTime null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CustomerConsent | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

