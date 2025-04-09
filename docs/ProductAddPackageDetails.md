# ProductAddPackageDetails
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MeasureUnit** | **String** |  | [optional] 
**WeighUnit** | **String** |  | [optional] 
**PackageDepth** | **Decimal** |  | [optional] 
**PackageLength** | **Decimal** |  | [optional] 
**PackageWidth** | **Decimal** |  | [optional] 
**WeightMajor** | **Decimal** |  | [optional] 
**WeightMinor** | **Decimal** |  | [optional] 
**ShippingPackage** | **String** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddPackageDetails = Initialize-PSOpenAPIToolsProductAddPackageDetails  -MeasureUnit null `
 -WeighUnit null `
 -PackageDepth null `
 -PackageLength null `
 -PackageWidth null `
 -WeightMajor null `
 -WeightMinor null `
 -ShippingPackage null
```

- Convert the resource to JSON
```powershell
$ProductAddPackageDetails | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

