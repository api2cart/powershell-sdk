# BasketLiveShippingService
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Callback** | **String** |  | [optional] 
**CallbackErrCnt** | **Int32** |  | [optional] 
**EnabledOnStore** | **Boolean** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$BasketLiveShippingService = Initialize-PSOpenAPIToolsBasketLiveShippingService  -Id null `
 -Name null `
 -Callback null `
 -CallbackErrCnt null `
 -EnabledOnStore null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$BasketLiveShippingService | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

