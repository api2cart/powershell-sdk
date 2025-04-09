# OrderItemOption
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OptionId** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Value** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**Weight** | **Decimal** |  | [optional] 
**Type** | **String** |  | [optional] 
**ProductOptionValueId** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderItemOption = Initialize-PSOpenAPIToolsOrderItemOption  -OptionId null `
 -Name null `
 -Value null `
 -Price null `
 -Weight null `
 -Type null `
 -ProductOptionValueId null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderItemOption | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

