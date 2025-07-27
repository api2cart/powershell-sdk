# ProductVariantAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **String** | Defines product&#39;s id where the variant has to be added | [optional] 
**Attributes** | [**ProductVariantAddAttributesInner[]**](ProductVariantAddAttributesInner.md) | Defines variant&#39;s attributes list | [optional] 
**Name** | **String** | Defines variant&#39;s name that has to be added | [optional] 
**Model** | **String** | Specifies variant&#39;s model that has to be added | 
**Description** | **String** | Specifies variant&#39;s description | [optional] 
**ShortDescription** | **String** | Defines short description | [optional] 
**AvailableForView** | **Boolean** | Specifies the set of visible/invisible product&#39;s variants for users | [optional] [default to $true]
**AvailableForSale** | **Boolean** | Specifies the set of visible/invisible product&#39;s variants for sale | [optional] [default to $true]
**IsVirtual** | **Boolean** | Defines whether the product is virtual | [optional] [default to $false]
**IsDefault** | **Boolean** | Defines as a default variant | [optional] 
**StoreId** | **String** | Add variants specified by store id | [optional] 
**StoresIds** | **String** | Assign variant to the stores that is specified by comma-separated stores&#39; id | [optional] 
**LangId** | **String** | Language id | [optional] 
**Price** | **Decimal** | Defines new product&#39;s variant price | [optional] 
**OldPrice** | **Decimal** | Defines product&#39;s old price | [optional] 
**CostPrice** | **Decimal** | Defines new product&#39;s cost price | [optional] 
**SpecialPrice** | **Decimal** | Specifies variant&#39;s model that has to be added | [optional] 
**SpriceCreate** | **String** | Defines the date of special price creation | [optional] 
**SpriceModified** | **String** | Defines the date of special price modification | [optional] 
**SpriceExpire** | **String** | Defines the term of special price offer duration | [optional] 
**TierPrices** | [**ProductAddTierPricesInner[]**](ProductAddTierPricesInner.md) | Defines product&#39;s tier prices | [optional] 
**Quantity** | **Decimal** | Defines product variant&#39;s quantity that has to be added | [optional] [default to 0]
**WarehouseId** | **String** | This parameter is used for selecting a warehouse where you need to set/modify a product quantity. | [optional] 
**InStock** | **Boolean** | Set stock status | [optional] 
**BackorderStatus** | **String** | Set backorder status | [optional] 
**ManageStock** | **Boolean** | Defines inventory tracking for product variant | [optional] 
**LowStockThreshold** | **Decimal** | Specify the quantity threshold below which the product is considered low in stock | [optional] 
**Weight** | **Decimal** | Weight | [optional] [default to 0]
**Width** | **Decimal** | Defines product&#39;s width | [optional] 
**Height** | **Decimal** | Defines product&#39;s height | [optional] 
**Length** | **Decimal** | Defines product&#39;s length | [optional] 
**WeightUnit** | **String** | Weight Unit | [optional] 
**Sku** | **String** | Defines variant&#39;s sku that has to be added | [optional] 
**Barcode** | **String** | A barcode is a unique code composed of numbers used as a product identifier. | [optional] 
**Gtin** | **String** | Global Trade Item Number. An GTIN is an identifier for trade items. | [optional] 
**Upc** | **String** | Universal Product Code. A UPC (UPC-A) is a commonly used identifer for many different products. | [optional] 
**Ean** | **String** | European Article Number. An EAN is a unique 8 or 13-digit identifier that many industries (such as book publishers) use to identify products. | [optional] 
**Mpn** | **String** | Manufacturer Part Number. A MPN is an identifier of a particular part design or material used. | [optional] 
**Isbn** | **String** | International Standard Book Number. An ISBN is a unique identifier for books. | [optional] 
**Manufacturer** | **String** | Specifies the product variant&#39;s manufacturer | [optional] 
**CreatedAt** | **String** | Defines the date of entity creation | [optional] 
**MetaTitle** | **String** | Defines unique meta title for each entity | [optional] 
**MetaKeywords** | **String** | Defines unique meta keywords for each entity | [optional] 
**MetaDescription** | **String** | Defines unique meta description of a entity | [optional] 
**Url** | **String** | Defines unique product variant&#39;s URL | [optional] 
**TaxClassId** | **String** | Defines tax classes where entity has to be added | [optional] 
**Taxable** | **Boolean** | Specifies whether a tax is charged | [optional] [default to $true]
**FixedCostShippingPrice** | **Decimal** | Specifies fixed cost shipping price | [optional] 
**IsFreeShipping** | **Boolean** | Specifies variant&#39;s free shipping flag that has to be added | [optional] 
**CountryOfOrigin** | **String** | The country where the inventory item was made | [optional] 
**HarmonizedSystemCode** | **String** | Harmonized System Code. An HSC is a 6-digit identifier that allows participating countries to classify traded goods on a common basis for customs purposes | [optional] 
**MarketplaceItemProperties** | **String** | String containing the JSON representation of the supplied data | [optional] 
**ClearCache** | **Boolean** | Is cache clear required | [optional] [default to $true]

## Examples

- Prepare the resource
```powershell
$ProductVariantAdd = Initialize-PSOpenAPIToolsProductVariantAdd  -ProductId 10 `
 -Attributes null `
 -Name Bag Green XXL `
 -Model bag_01 `
 -Description Product variant `
 -ShortDescription Short description. This is very short description `
 -AvailableForView false `
 -AvailableForSale false `
 -IsVirtual false `
 -IsDefault true `
 -StoreId 1 `
 -StoresIds 1,2 `
 -LangId 3 `
 -Price 99.9 `
 -OldPrice 99.9 `
 -CostPrice 65.9 `
 -SpecialPrice 56.9 `
 -SpriceCreate 2018-08-25 23:56:12 `
 -SpriceModified 2018-12-05 13:46:20 `
 -SpriceExpire 2018-08-25 23:56:12 `
 -TierPrices null `
 -Quantity 6 `
 -WarehouseId 1 `
 -InStock true `
 -BackorderStatus true `
 -ManageStock false `
 -LowStockThreshold 1 `
 -Weight 23.69 `
 -Width 56.12 `
 -Height 56.12 `
 -Length 56.12 `
 -WeightUnit lb `
 -Sku bag_01 `
 -Barcode 9770317847001 `
 -Gtin 12345678912345 `
 -Upc 9770317847001 `
 -Ean 5901234123457 `
 -Mpn 9770317847001 `
 -Isbn 9783161484100 `
 -Manufacturer Samsung `
 -CreatedAt 2014-08-09 13:13:13 `
 -MetaTitle category,test `
 -MetaKeywords category,test `
 -MetaDescription category,test `
 -Url /product_variant_slug `
 -TaxClassId 9 `
 -Taxable false `
 -FixedCostShippingPrice 5.5 `
 -IsFreeShipping true `
 -CountryOfOrigin 123456 `
 -HarmonizedSystemCode 123456 `
 -MarketplaceItemProperties {&quot;color&quot;:[&quot;Silver&quot;],&quot;manufacturer&quot;:&quot;Philips&quot;,&quot;features&quot;:[&quot;3 way&quot;],&quot;countPerPack&quot;:1,&quot;watts&quot;:{&quot;unit&quot;:&quot;W&quot;,&quot;measure&quot;:40}} `
 -ClearCache false
```

- Convert the resource to JSON
```powershell
$ProductVariantAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

