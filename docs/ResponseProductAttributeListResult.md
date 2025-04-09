# ResponseProductAttributeListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Attribute** | [**ProductAttribute[]**](ProductAttribute.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseProductAttributeListResult = Initialize-PSOpenAPIToolsResponseProductAttributeListResult  -Attribute null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseProductAttributeListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

