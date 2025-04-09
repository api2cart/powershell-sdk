# ProductAddSpecificsInnerBookingDetails
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Location** | **String** |  | 
**Type** | **String** |  | 
**SessionDuration** | **Int32** |  | [optional] 
**SessionGap** | **Int32** |  | [optional] 
**SessionsCount** | **Int32** |  | 
**TimeStrictValue** | **Decimal** |  | 
**TimeStrictType** | **String** |  | [default to "days"]
**Availabilities** | [**ProductAddSpecificsInnerBookingDetailsAvailabilitiesInner[]**](ProductAddSpecificsInnerBookingDetailsAvailabilitiesInner.md) |  | 
**Overrides** | [**ProductAddSpecificsInnerBookingDetailsOverridesInner[]**](ProductAddSpecificsInnerBookingDetailsOverridesInner.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddSpecificsInnerBookingDetails = Initialize-PSOpenAPIToolsProductAddSpecificsInnerBookingDetails  -Location null `
 -Type null `
 -SessionDuration null `
 -SessionGap null `
 -SessionsCount null `
 -TimeStrictValue null `
 -TimeStrictType null `
 -Availabilities null `
 -Overrides null
```

- Convert the resource to JSON
```powershell
$ProductAddSpecificsInnerBookingDetails | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

