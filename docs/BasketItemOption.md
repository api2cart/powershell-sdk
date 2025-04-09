# BasketItemOption
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**ValueId** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Value** | **String** |  | [optional] 
**UsedInCombination** | **Boolean** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$BasketItemOption = Initialize-PSOpenAPIToolsBasketItemOption  -Id null `
 -ValueId null `
 -Name null `
 -Value null `
 -UsedInCombination null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$BasketItemOption | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

