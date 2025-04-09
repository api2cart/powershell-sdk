# ProductVariantUpdate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**StoreId** | **String** | Defines store id where the variant should be found | [optional] 
**Id** | **String** | Defines variant update specified by variant id | [optional] 
**ProductId** | **String** | Defines product&#39;s id where the variant has to be updated | [optional] 
**WarehouseId** | **String** | This parameter is used for selecting a warehouse where you need to set/modify a product quantity. | [optional] 
**ReserveQuantity** | **Decimal** | This parameter allows to reserve/unreserve product variants quantity. | [optional] 
**Quantity** | **Decimal** | Defines new products&#39; variants quantity | [optional] 
**IncreaseQuantity** | **Decimal** | Defines the incremental changes in product quantity | [optional] [default to 0]
**ReduceQuantity** | **Decimal** | Defines the decrement changes in product quantity | [optional] [default to 0]
**Price** | **Decimal** | Defines new product&#39;s variant price | [optional] 
**SpecialPrice** | **Decimal** | Defines new product&#39;s variant special price | [optional] 
**RetailPrice** | **Decimal** | Defines new product&#39;s retail price | [optional] 
**OldPrice** | **Decimal** | Defines product&#39;s old price | [optional] 
**CostPrice** | **Decimal** | Defines new product&#39;s cost price | [optional] 
**FixedCostShippingPrice** | **Decimal** | Specifies fixed cost shipping price | [optional] 
**SpriceCreate** | **String** | Defines the date of special price creation | [optional] 
**SpriceExpire** | **String** | Defines the term of special price offer duration | [optional] 
**ManageStock** | **Boolean** | Defines inventory tracking for product variant | [optional] 
**InStock** | **Boolean** | Set stock status | [optional] 
**Name** | **String** | Defines variant&#39;s name that has to be updated | [optional] 
**Description** | **String** | Specifies variant&#39;s description | [optional] 
**Sku** | **String** | Defines new product&#39;s variant sku | [optional] 
**MetaTitle** | **String** | Defines unique meta title for each entity | [optional] 
**MetaDescription** | **String** | Defines unique meta description of a entity | [optional] 
**MetaKeywords** | **String** | Defines unique meta keywords for each entity | [optional] 
**ShortDescription** | **String** | Defines short description | [optional] 
**Visible** | **String** | Set visibility status | [optional] 
**Status** | **String** | Defines product variant&#39;s status | [optional] 
**BackorderStatus** | **String** | Set backorder status | [optional] 
**Weight** | **Decimal** | Weight | [optional] [default to 0]
**Barcode** | **String** | A barcode is a unique code composed of numbers used as a product identifier. | [optional] 
**Reindex** | **Boolean** | Is reindex required | [optional] [default to $true]
**Taxable** | **Boolean** | Specifies whether a tax is charged | [optional] [default to $true]
**Options** | [**ProductVariantUpdateOptionsInner[]**](ProductVariantUpdateOptionsInner.md) | Defines variant&#39;s options list | [optional] 
**HarmonizedSystemCode** | **String** | Harmonized System Code. An HSC is a 6-digit identifier that allows participating countries to classify traded goods on a common basis for customs purposes | [optional] 
**CountryOfOrigin** | **String** | The country where the inventory item was made | [optional] 
**Width** | **Decimal** | Defines product&#39;s width | [optional] 
**WeightUnit** | **String** | Weight Unit | [optional] 
**Height** | **Decimal** | Defines product&#39;s height | [optional] 
**Length** | **Decimal** | Defines product&#39;s length | [optional] 
**Gtin** | **String** | Global Trade Item Number. An GTIN is an identifier for trade items. | [optional] 
**ClearCache** | **Boolean** | Is cache clear required | [optional] [default to $true]
**LangId** | **String** | Language id | [optional] 
**Model** | **String** | Specifies variant&#39;s model that has to be added | [optional] 
**AvailableForSale** | **Boolean** | Specifies the set of visible/invisible product&#39;s variants for sale | [optional] [default to $true]
**Upc** | **String** | Universal Product Code. A UPC (UPC-A) is a commonly used identifer for many different products. | [optional] 
**Mpn** | **String** | Manufacturer Part Number. A MPN is an identifier of a particular part design or material used. | [optional] 
**Ean** | **String** | European Article Number. An EAN is a unique 8 or 13-digit identifier that many industries (such as book publishers) use to identify products. | [optional] 
**Isbn** | **String** | International Standard Book Number. An ISBN is a unique identifier for books. | [optional] 
**Avail** | **Boolean** | Defines category&#39;s visibility status | [optional] [default to $true]
**IsDefault** | **Boolean** | Defines as a default variant | [optional] 
**IsFreeShipping** | **Boolean** | Specifies variant&#39;s free shipping flag that has to be added | [optional] 
**TaxClassId** | **String** | Defines tax classes where entity has to be added | [optional] 
**IsVirtual** | **Boolean** | Defines whether the product is virtual | [optional] [default to $false]

## Examples

- Prepare the resource
```powershell
$ProductVariantUpdate = Initialize-PSOpenAPIToolsProductVariantUpdate  -StoreId 1 `
 -Id 10 `
 -ProductId 10 `
 -WarehouseId 1 `
 -ReserveQuantity 1 `
 -Quantity 6 `
 -IncreaseQuantity 4 `
 -ReduceQuantity 4 `
 -Price 99.9 `
 -SpecialPrice 56.9 `
 -RetailPrice 6.9 `
 -OldPrice 99.9 `
 -CostPrice 65.9 `
 -FixedCostShippingPrice 5.5 `
 -SpriceCreate 2018-08-25 23:56:12 `
 -SpriceExpire 2018-08-25 23:56:12 `
 -ManageStock false `
 -InStock true `
 -Name Bag Green L `
 -Description Product variant `
 -Sku bag_01 `
 -MetaTitle category,test `
 -MetaDescription category,test `
 -MetaKeywords category,test `
 -ShortDescription Short description. This is very short description `
 -Visible catalog `
 -Status disabled `
 -BackorderStatus true `
 -Weight 23.69 `
 -Barcode 9770317847001 `
 -Reindex false `
 -Taxable false `
 -Options null `
 -HarmonizedSystemCode 123456 `
 -CountryOfOrigin 123456 `
 -Width 56.12 `
 -WeightUnit lb `
 -Height 56.12 `
 -Length 56.12 `
 -Gtin 12345678912345 `
 -ClearCache false `
 -LangId 3 `
 -Model bag_01 `
 -AvailableForSale false `
 -Upc 9770317847001 `
 -Mpn 9770317847001 `
 -Ean 5901234123457 `
 -Isbn 9783161484100 `
 -Avail false `
 -IsDefault true `
 -IsFreeShipping true `
 -TaxClassId 9 `
 -IsVirtual false
```

- Convert the resource to JSON
```powershell
$ProductVariantUpdate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

