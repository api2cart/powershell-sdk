# OrderCalculateTax
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | **String** |  | [optional] 
**Rate** | **Decimal** |  | [optional] 
**Value** | **Decimal** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderCalculateTax = Initialize-PSOpenAPIToolsOrderCalculateTax  -Code null `
 -Rate null `
 -Value null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderCalculateTax | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

