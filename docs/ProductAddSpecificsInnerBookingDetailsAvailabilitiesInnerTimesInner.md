# ProductAddSpecificsInnerBookingDetailsAvailabilitiesInnerTimesInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**VarFrom** | **String** | The starting time of the of available booking slot in 24 hours format. Required if &lt;code&gt;type&#x3D;date_time&lt;/code&gt; | 
**To** | **String** | The ending time of the of available booking slot in 24 hours format. Required if &lt;code&gt;type&#x3D;date_time&lt;/code&gt; | 

## Examples

- Prepare the resource
```powershell
$ProductAddSpecificsInnerBookingDetailsAvailabilitiesInnerTimesInner = Initialize-PSOpenAPIToolsProductAddSpecificsInnerBookingDetailsAvailabilitiesInnerTimesInner  -VarFrom null `
 -To null
```

- Convert the resource to JSON
```powershell
$ProductAddSpecificsInnerBookingDetailsAvailabilitiesInnerTimesInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

