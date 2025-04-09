# ResponseAttributeGroupListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Group** | [**StoreAttributeGroup[]**](StoreAttributeGroup.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseAttributeGroupListResult = Initialize-PSOpenAPIToolsResponseAttributeGroupListResult  -Group null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseAttributeGroupListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

