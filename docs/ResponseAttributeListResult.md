# ResponseAttributeListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributesCount** | **Int32** |  | [optional] 
**Attribute** | [**StoreAttribute[]**](StoreAttribute.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseAttributeListResult = Initialize-PSOpenAPIToolsResponseAttributeListResult  -AttributesCount null `
 -Attribute null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseAttributeListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

