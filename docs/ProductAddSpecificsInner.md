# ProductAddSpecificsInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **String** |  | [optional] 
**Value** | **String** |  | [optional] 
**Values** | **String[]** |  | [optional] 
**UsedForVariations** | **Boolean** |  | [optional] [default to $false]
**ScaleId** | **Int32** |  | [optional] 
**FoodDetails** | [**ProductAddSpecificsInnerFoodDetails**](ProductAddSpecificsInnerFoodDetails.md) |  | [optional] 
**GroupProductsDetails** | [**ProductAddSpecificsInnerGroupProductsDetailsInner[]**](ProductAddSpecificsInnerGroupProductsDetailsInner.md) |  | [optional] 
**BookingDetails** | [**ProductAddSpecificsInnerBookingDetails**](ProductAddSpecificsInnerBookingDetails.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddSpecificsInner = Initialize-PSOpenAPIToolsProductAddSpecificsInner  -Name null `
 -Value null `
 -Values null `
 -UsedForVariations null `
 -ScaleId null `
 -FoodDetails null `
 -GroupProductsDetails null `
 -BookingDetails null
```

- Convert the resource to JSON
```powershell
$ProductAddSpecificsInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

