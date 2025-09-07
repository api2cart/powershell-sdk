# OrderCalculateDiscount
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | **String** |  | [optional] 
**Value** | **Decimal** |  | [optional] 
**Type** | **String** |  | [optional] 
**FreeShipping** | **Boolean** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderCalculateDiscount = Initialize-PSOpenAPIToolsOrderCalculateDiscount  -Code null `
 -Value null `
 -Type null `
 -FreeShipping null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderCalculateDiscount | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

