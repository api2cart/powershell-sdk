# ResponseOrderPreestimateShippingListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PreestimateShippingsCount** | **Int32** |  | [optional] 
**PreestimateShippings** | [**OrderPreestimateShipping[]**](OrderPreestimateShipping.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseOrderPreestimateShippingListResult = Initialize-PSOpenAPIToolsResponseOrderPreestimateShippingListResult  -PreestimateShippingsCount null `
 -PreestimateShippings null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseOrderPreestimateShippingListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

