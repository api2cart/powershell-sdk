# ResponseOrderShipmentListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ShipmentCount** | **Int32** |  | [optional] 
**Shipment** | [**Shipment[]**](Shipment.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseOrderShipmentListResult = Initialize-PSOpenAPIToolsResponseOrderShipmentListResult  -ShipmentCount null `
 -Shipment null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseOrderShipmentListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

