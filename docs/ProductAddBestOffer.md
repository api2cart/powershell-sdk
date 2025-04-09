# ProductAddBestOffer
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MinimumOfferPrice** | **Decimal** |  | [optional] 
**AutoAcceptPrice** | **Decimal** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddBestOffer = Initialize-PSOpenAPIToolsProductAddBestOffer  -MinimumOfferPrice null `
 -AutoAcceptPrice null
```

- Convert the resource to JSON
```powershell
$ProductAddBestOffer | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

