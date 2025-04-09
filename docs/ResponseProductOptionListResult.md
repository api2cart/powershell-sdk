# ResponseProductOptionListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Option** | [**ProductOption[]**](ProductOption.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseProductOptionListResult = Initialize-PSOpenAPIToolsResponseProductOptionListResult  -Option null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseProductOptionListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

