# StoreAttributeAttributeSet
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**AssignedAttributeIds** | **String[]** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$StoreAttributeAttributeSet = Initialize-PSOpenAPIToolsStoreAttributeAttributeSet  -Id null `
 -Name null `
 -AssignedAttributeIds null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$StoreAttributeAttributeSet | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

