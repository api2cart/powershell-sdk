# StoreAttributeGroup
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Position** | **Int32** |  | [optional] 
**AttributeSetId** | **String** |  | [optional] 
**AssignedAttributeIds** | **String[]** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$StoreAttributeGroup = Initialize-PSOpenAPIToolsStoreAttributeGroup  -Id null `
 -Name null `
 -Position null `
 -AttributeSetId null `
 -AssignedAttributeIds null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$StoreAttributeGroup | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

