# Discount
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**ModifierType** | **String** |  | [optional] 
**Value** | **Decimal** |  | [optional] 
**FromTime** | **String** |  | [optional] 
**ToTime** | **String** |  | [optional] 
**CustomerGroupIds** | **String** |  | [optional] 
**SortOrder** | **Int32** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Discount = Initialize-PSOpenAPIToolsDiscount  -Id null `
 -Name null `
 -ModifierType null `
 -Value null `
 -FromTime null `
 -ToTime null `
 -CustomerGroupIds null `
 -SortOrder null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Discount | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

