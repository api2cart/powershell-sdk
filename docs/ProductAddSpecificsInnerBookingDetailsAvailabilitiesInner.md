# ProductAddSpecificsInnerBookingDetailsAvailabilitiesInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Day** | **String** |  | 
**IsAvailable** | **Boolean** |  | [optional] [default to $true]
**Times** | [**ProductAddSpecificsInnerBookingDetailsAvailabilitiesInnerTimesInner[]**](ProductAddSpecificsInnerBookingDetailsAvailabilitiesInnerTimesInner.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddSpecificsInnerBookingDetailsAvailabilitiesInner = Initialize-PSOpenAPIToolsProductAddSpecificsInnerBookingDetailsAvailabilitiesInner  -Day null `
 -IsAvailable null `
 -Times null
```

- Convert the resource to JSON
```powershell
$ProductAddSpecificsInnerBookingDetailsAvailabilitiesInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

