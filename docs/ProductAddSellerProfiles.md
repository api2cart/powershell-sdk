# ProductAddSellerProfiles
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ShippingProfileId** | **String** |  | [optional] 
**PaymentProfileId** | **String** |  | [optional] 
**ReturnProfileId** | **String** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddSellerProfiles = Initialize-PSOpenAPIToolsProductAddSellerProfiles  -ShippingProfileId null `
 -PaymentProfileId null `
 -ReturnProfileId null
```

- Convert the resource to JSON
```powershell
$ProductAddSellerProfiles | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

