# ResponseAttributeAttributesetListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeSet** | [**StoreAttributeAttributeSet[]**](StoreAttributeAttributeSet.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseAttributeAttributesetListResult = Initialize-PSOpenAPIToolsResponseAttributeAttributesetListResult  -AttributeSet null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseAttributeAttributesetListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

