# ProductUpdate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** | Defines product id that has to be updated | [optional] 
**Model** | **String** | Defines product model that has to be updated | [optional] 
**Sku** | **String** | Defines new product&#39;s sku | [optional] 
**Name** | **String** | Defines product&#39;s name that has to be updated | [optional] 
**Description** | **String** | Defines new product&#39;s description | [optional] 
**ShortDescription** | **String** | Defines short description | [optional] 
**Price** | **Decimal** | Defines new product&#39;s price | [optional] 
**OldPrice** | **Decimal** | Defines product&#39;s old price | [optional] 
**SpecialPrice** | **Decimal** | Defines new product&#39;s special price | [optional] 
**SpriceCreate** | **String** | Defines the date of special price creation | [optional] 
**SpriceExpire** | **String** | Defines the term of special price offer duration | [optional] 
**CostPrice** | **Decimal** | Defines new product&#39;s cost price | [optional] 
**FixedCostShippingPrice** | **Decimal** | Specifies product&#39;s fixed cost shipping price | [optional] 
**RetailPrice** | **Decimal** | Defines new product&#39;s retail price | [optional] 
**TierPrices** | [**ProductAddTierPricesInner[]**](ProductAddTierPricesInner.md) | Defines product&#39;s tier prices | [optional] 
**ReservePrice** | **Decimal** | Defines reserve price value | [optional] 
**BuyitnowPrice** | **Decimal** | Defines buy it now value | [optional] 
**Taxable** | **Boolean** | Specifies whether a tax is charged | [optional] [default to $true]
**TaxClassId** | **String** | Defines tax classes where entity has to be added | [optional] 
**Type** | **String** | Defines product&#39;s type | [optional] 
**Status** | **String** | Defines product&#39;s status | [optional] 
**Condition** | **String** | The human-readable label for the condition (e.g., &quot;&quot;New&quot;&quot;). | [optional] 
**Visible** | **String** | Set visibility status | [optional] 
**InStock** | **Boolean** | Set stock status | [optional] 
**Avail** | **Boolean** | Defines category&#39;s visibility status | [optional] [default to $true]
**AvailFrom** | **String** | Allows to schedule a time in the future that the item becomes available. The value should be greater than the current date and time. | [optional] 
**ProductClass** | **String** | A categorization for the product | [optional] 
**AvailableForView** | **Boolean** | Specifies the set of visible/invisible products for users | [optional] 
**StoresIds** | **String** | Assign product to the stores that is specified by comma-separated stores&#39; id | [optional] 
**StoreId** | **String** | Defines store id where the product should be found | [optional] 
**LangId** | **String** | Language id | [optional] 
**Quantity** | **Decimal** | Defines new product&#39;s quantity | [optional] 
**ReserveQuantity** | **Decimal** | This parameter allows to reserve/unreserve product quantity. | [optional] 
**ManageStock** | **Boolean** | Defines inventory tracking for product | [optional] 
**BackorderStatus** | **String** | Set backorder status | [optional] 
**IncreaseQuantity** | **Decimal** | Defines the incremental changes in product quantity | [optional] 
**ReduceQuantity** | **Decimal** | Defines the decrement changes in product quantity | [optional] 
**WarehouseId** | **String** | This parameter is used for selecting a warehouse where you need to set/modify a product quantity. | [optional] 
**Weight** | **Decimal** | Weight | [optional] 
**WeightUnit** | **String** | Weight Unit | [optional] 
**Height** | **Decimal** | Defines product&#39;s height | [optional] 
**Length** | **Decimal** | Defines product&#39;s length | [optional] 
**Width** | **Decimal** | Defines product&#39;s width | [optional] 
**DimensionsUnit** | **String** | Weight Unit | [optional] 
**IsVirtual** | **Boolean** | Defines whether the product is virtual | [optional] [default to $false]
**IsFreeShipping** | **Boolean** | Specifies product free shipping flag that has to be updated | [optional] 
**Gtin** | **String** | Global Trade Item Number. An GTIN is an identifier for trade items. | [optional] 
**Upc** | **String** | Universal Product Code. A UPC (UPC-A) is a commonly used identifer for many different products. | [optional] 
**Mpn** | **String** | Manufacturer Part Number. A MPN is an identifier of a particular part design or material used. | [optional] 
**Ean** | **String** | European Article Number. An EAN is a unique 8 or 13-digit identifier that many industries (such as book publishers) use to identify products. | [optional] 
**Isbn** | **String** | International Standard Book Number. An ISBN is a unique identifier for books. | [optional] 
**Barcode** | **String** | A barcode is a unique code composed of numbers used as a product identifier. | [optional] 
**Manufacturer** | **String** | Defines product&#39;s manufacturer | [optional] 
**ManufacturerId** | **String** | Defines product&#39;s manufacturer by manufacturer_id | [optional] 
**CategoriesIds** | **String** | Defines product add that is specified by comma-separated categories id | [optional] 
**RelatedProductsIds** | **String** | Defines product related products ids that has to be updated | [optional] 
**UpSellProductsIds** | **String** | Defines product up-sell products ids that has to be updated | [optional] 
**CrossSellProductsIds** | **String** | Defines product cross-sells products ids that has to be updated | [optional] 
**MetaTitle** | **String** | Defines unique meta title for each entity | [optional] 
**MetaKeywords** | **String** | Defines unique meta keywords for each entity | [optional] 
**MetaDescription** | **String** | Defines unique meta description of a entity | [optional] 
**SeoUrl** | **String** | Defines unique URL for SEO | [optional] 
**SearchKeywords** | **String** | Defines unique search keywords | [optional] 
**Tags** | **String** | Product tags | [optional] 
**DeliveryCode** | **String** | The delivery promise that applies to offer | [optional] 
**PackageDetails** | [**ProductAddPackageDetails**](ProductAddPackageDetails.md) |  | [optional] 
**CountryOfOrigin** | **String** | The country where the inventory item was made | [optional] 
**HarmonizedSystemCode** | **String** | Harmonized System Code. An HSC is a 6-digit identifier that allows participating countries to classify traded goods on a common basis for customs purposes | [optional] 
**ShippingTemplateId** | **Int32** | The numeric ID of the shipping template associated with the products in Etsy. You can find possible values in the &quot;&quot;cart.info&quot;&quot; API method response, in the field shipping_zones[]-&gt;id. | [optional] [default to 0]
**WhenMade** | **String** | An enumerated string for the era in which the maker made the product. | [optional] [default to "made_to_order"]
**IsSupply** | **Boolean** | If true, it indicates the product as a supply, otherwise it indicates that it is a finished product. | [optional] [default to $true]
**Downloadable** | **Boolean** | Defines whether the product is downloadable | [optional] [default to $false]
**Materials** | **String[]** | A list of material strings for materials used in the product. | [optional] 
**AutoRenew** | **Boolean** | When true, automatically renews a listing upon its expiration. | [optional] [default to $false]
**OnSale** | **Boolean** | Set whether the product on sale | [optional] [default to $false]
**ProductionPartnerIds** | **String** | Defines product production partner ids that has to be updated | [optional] 
**ManufacturerInfo** | [**ProductAddManufacturerInfo**](ProductAddManufacturerInfo.md) |  | [optional] 
**ReportRequestId** | **String** | Report request id | [optional] 
**DisableReportCache** | **Boolean** | Disable report cache for current request | [optional] [default to $false]
**Reindex** | **Boolean** | Is reindex required | [optional] [default to $true]
**ClearCache** | **Boolean** | Is cache clear required | [optional] [default to $true]
**CheckProcessStatus** | **Boolean** | Disable or enable check process status. Please note that the response will be slower due to additional requests to the store. | [optional] [default to $false]
**Specifics** | [**ProductAddSpecificsInner[]**](ProductAddSpecificsInner.md) | An array of Item Specific Name/Value pairs used by the seller to provide descriptive details of an item in a structured manner.         The list of possible specifications can be obtained using the category.info method (additional_fields-&gt;product_specifics).         &lt;b&gt;The structure of the parameter is different for specific platforms.&lt;/b&gt; | [optional] 
**ShopSectionId** | **Int32** | Add Shop Section Id | [optional] 
**PersonalizationDetails** | [**ProductAddPersonalizationDetails**](ProductAddPersonalizationDetails.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductUpdate = Initialize-PSOpenAPIToolsProductUpdate  -Id 10 `
 -Model bag_01 `
 -Sku bag_01 `
 -Name Pancil `
 -Description New product description `
 -ShortDescription Short description. This is very short description `
 -Price 99.9 `
 -OldPrice 99.9 `
 -SpecialPrice 56.9 `
 -SpriceCreate 2018-08-25 23:56:12 `
 -SpriceExpire 2018-08-25 23:56:12 `
 -CostPrice 65.9 `
 -FixedCostShippingPrice 5.5 `
 -RetailPrice 6.9 `
 -TierPrices null `
 -ReservePrice 65.9 `
 -BuyitnowPrice 65.9 `
 -Taxable false `
 -TaxClassId 9 `
 -Type simple `
 -Status disabled `
 -Condition Like New `
 -Visible search `
 -InStock true `
 -Avail false `
 -AvailFrom avail_from&#x3D;2029-10-25T15:54:37-0500 `
 -ProductClass Shirts `
 -AvailableForView false `
 -StoresIds 1,2 `
 -StoreId 1 `
 -LangId 3 `
 -Quantity 6 `
 -ReserveQuantity 1 `
 -ManageStock false `
 -BackorderStatus true `
 -IncreaseQuantity 4 `
 -ReduceQuantity 4 `
 -WarehouseId 1 `
 -Weight 23.69 `
 -WeightUnit lb `
 -Height 56.12 `
 -Length 56.12 `
 -Width 56.12 `
 -DimensionsUnit cm `
 -IsVirtual false `
 -IsFreeShipping true `
 -Gtin 12345678912345 `
 -Upc 9770317847001 `
 -Mpn 9770317847001 `
 -Ean 5901234123457 `
 -Isbn 9783161484100 `
 -Barcode 9770317847001 `
 -Manufacturer Samsung `
 -ManufacturerId 1 `
 -CategoriesIds 23,56 `
 -RelatedProductsIds 4,5 `
 -UpSellProductsIds 4,5 `
 -CrossSellProductsIds 4,5 `
 -MetaTitle category,test `
 -MetaKeywords category,test `
 -MetaDescription category,test `
 -SeoUrl some seo url `
 -SearchKeywords key1,key2,key3 `
 -Tags tag1,tag2 `
 -DeliveryCode 24uurs-23 `
 -PackageDetails null `
 -CountryOfOrigin 123456 `
 -HarmonizedSystemCode 123456 `
 -ShippingTemplateId 40256592690 `
 -WhenMade 2020_2025 `
 -IsSupply false `
 -Downloadable true `
 -Materials materials[0]&#x3D;Aluminum&amp;materials[1]&#x3D;Brass `
 -AutoRenew false `
 -OnSale false `
 -ProductionPartnerIds 4,5 `
 -ManufacturerInfo null `
 -ReportRequestId 105245017661 `
 -DisableReportCache false `
 -Reindex false `
 -ClearCache false `
 -CheckProcessStatus false `
 -Specifics null `
 -ShopSectionId &#x60;12345678&#x60; `
 -PersonalizationDetails null
```

- Convert the resource to JSON
```powershell
$ProductUpdate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

