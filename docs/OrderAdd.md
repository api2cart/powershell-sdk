# OrderAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** | Defines order&#39;s id | [optional] 
**OrderId** | **String** | Defines the order id if it is supported by the cart | [optional] 
**StoreId** | **String** | Defines store id where the order should be assigned | [optional] 
**ChannelId** | **String** | Channel ID | [optional] 
**OrderStatus** | **String** | Defines order status. | 
**FulfillmentStatus** | **String** | Create order with fulfillment status | [optional] 
**FinancialStatus** | **String** | Create order with financial status | [optional] 
**CustomerEmail** | **String** | Defines the customer specified by email for whom order has to be created | 
**CustomerFirstName** | **String** | Specifies customer&#39;s first name | [optional] 
**CustomerLastName** | **String** | Specifies customer’s last name | [optional] 
**CustomerPhone** | **String** | Specifies customer’s phone | [optional] 
**CustomerCountry** | **String** | Specifies customer&#39;s address ISO code or name of country | [optional] 
**CustomerBirthday** | **String** | Specifies customer’s birthday | [optional] 
**CustomerFax** | **String** | Specifies customer’s fax | [optional] 
**OrderPaymentMethod** | **String** | Defines order payment method.&lt;br/&gt;Setting order_payment_method on Shopify will also change financial_status field value to &#39;paid&#39; | [optional] 
**TransactionId** | **String** | Payment transaction id | [optional] 
**Currency** | **String** | Currency code of order | [optional] 
**Date** | **String** | Specifies an order creation date in format Y-m-d H:i:s | [optional] 
**DateModified** | **String** | Specifies order&#39;s  modification date | [optional] 
**DateFinished** | **String** | Specifies order&#39;s  finished date | [optional] 
**BillFirstName** | **String** | Specifies billing first name | 
**BillLastName** | **String** | Specifies billing last name | 
**BillAddress1** | **String** | Specifies first billing address | 
**BillAddress2** | **String** | Specifies second billing address | [optional] 
**BillCity** | **String** | Specifies billing city | 
**BillPostcode** | **String** | Specifies billing postcode | 
**BillState** | **String** | Specifies billing state code | 
**BillCountry** | **String** | Specifies billing country code | 
**BillCompany** | **String** | Specifies billing company | [optional] 
**BillPhone** | **String** | Specifies billing phone | [optional] 
**BillFax** | **String** | Specifies billing fax | [optional] 
**ShippFirstName** | **String** | Specifies shipping first name | [optional] 
**ShippLastName** | **String** | Specifies shipping last name | [optional] 
**ShippAddress1** | **String** | Specifies first shipping address | [optional] 
**ShippAddress2** | **String** | Specifies second address line of a shipping street address | [optional] 
**ShippCity** | **String** | Specifies shipping city | [optional] 
**ShippPostcode** | **String** | Specifies shipping postcode | [optional] 
**ShippState** | **String** | Specifies shipping state code | [optional] 
**ShippCountry** | **String** | Specifies shipping country code | [optional] 
**ShippCompany** | **String** | Specifies shipping company | [optional] 
**ShippPhone** | **String** | Specifies shipping phone | [optional] 
**ShippFax** | **String** | Specifies shipping fax | [optional] 
**SubtotalPrice** | **Decimal** | Total price of all ordered products multiplied by their number, excluding tax, shipping price and discounts | [optional] 
**TaxPrice** | **Decimal** | The value of tax cost for order | [optional] [default to 0]
**TotalPrice** | **Decimal** | Defines order&#39;s total price | [optional] 
**TotalPaid** | **Decimal** | Defines total paid amount for the order | [optional] 
**TotalWeight** | **Int32** | Defines the sum of all line item weights in grams for the order | [optional] 
**PricesIncTax** | **Boolean** | Indicates whether prices and subtotal includes tax. | [optional] [default to $false]
**ShippingPrice** | **Decimal** | Specifies order&#39;s shipping price | [optional] [default to 0]
**ShippingTax** | **Decimal** | Specifies order&#39;s shipping price tax | [optional] 
**Discount** | **Decimal** | Specifies order&#39;s discount | [optional] 
**CouponDiscount** | **Decimal** | Specifies order&#39;s coupon discount | [optional] 
**GiftCertificateDiscount** | **Decimal** | Discounts for order with gift certificates | [optional] 
**OrderShippingMethod** | **String** | Defines order shipping method | [optional] 
**CarrierId** | **String** | Defines tracking carrier id | [optional] 
**WarehouseId** | **String** | This parameter is used for selecting a warehouse where you need to set/modify a product quantity. | [optional] 
**Coupons** | **String[]** | Coupons that will be applied to order | [optional] 
**Tags** | **String** | Order tags | [optional] 
**Comment** | **String** | Specifies order comment | [optional] 
**AdminComment** | **String** | Specifies admin&#39;s order comment | [optional] 
**AdminPrivateComment** | **String** | Specifies private admin&#39;s order comment | [optional] 
**SendNotifications** | **Boolean** | Send notifications to customer after order was created | [optional] [default to $false]
**SendAdminNotifications** | **Boolean** | Notify admin when new order was created. | [optional] [default to $false]
**ExternalSource** | **String** | Identifying the system used to generate the order | [optional] 
**InventoryBehaviour** | **String** | The behaviour to use when updating inventory.&lt;hr&gt;&lt;div style&#x3D;&quot;&quot;font-style:normal&quot;&quot;&gt;Values description:&lt;div style&#x3D;&quot;&quot;margin-left: 2%; padding-top: 2%&quot;&quot;&gt;&lt;div style&#x3D;&quot;&quot;font-size:85%&quot;&quot;&gt;&lt;b&gt;bypass&lt;/b&gt; &#x3D; Do not claim inventory &lt;/br&gt;&lt;/br&gt;&lt;b&gt;decrement_ignoring_policy&lt;/b&gt; &#x3D; Ignore the product&#39;s &lt;/br&gt; inventory policy and claim amounts&lt;/br&gt;&lt;/br&gt;&lt;b&gt;decrement_obeying_policy&lt;/b&gt; &#x3D;  Obey the product&#39;s &lt;/br&gt; inventory policy.&lt;/br&gt;&lt;/br&gt;&lt;/div&gt;&lt;/div&gt;&lt;/div&gt; | [optional] [default to "bypass"]
**CreateInvoice** | **Boolean** | Defines whether the invoice is created automatically along with the order | [optional] [default to $false]
**NoteAttributes** | [**OrderAddNoteAttributesInner[]**](OrderAddNoteAttributesInner.md) | Defines note attributes | [optional] 
**ClearCache** | **Boolean** | Is cache clear required | [optional] [default to $true]
**Origin** | **String** | The source of the order | [optional] 
**FeePrice** | **Decimal** | Specifies refund&#39;s fee price | [optional] 
**OrderItem** | [**OrderAddOrderItemInner[]**](OrderAddOrderItemInner.md) |  | 

## Examples

- Prepare the resource
```powershell
$OrderAdd = Initialize-PSOpenAPIToolsOrderAdd  -Id 10 `
 -OrderId 25 `
 -StoreId 1 `
 -ChannelId 1 `
 -OrderStatus Completed `
 -FulfillmentStatus fulfilled `
 -FinancialStatus paid `
 -CustomerEmail jubari@hannsgroup.com `
 -CustomerFirstName John `
 -CustomerLastName Smith `
 -CustomerPhone 88008547457 `
 -CustomerCountry US `
 -CustomerBirthday 1990-12-03 `
 -CustomerFax 5656598 `
 -OrderPaymentMethod PayPal `
 -TransactionId d41d8cd98f00b204e9800998ecf8427e `
 -Currency USD `
 -Date 2012-09-25 19:40:00 `
 -DateModified 2014-05-05 05:05:00 `
 -DateFinished 2014-06-05 05:05:00 `
 -BillFirstName Adam `
 -BillLastName Smith `
 -BillAddress1 Green str. 35 `
 -BillAddress2 Red str, 2 `
 -BillCity Chicago `
 -BillPostcode 12345 `
 -BillState IL `
 -BillCountry US `
 -BillCompany Apple `
 -BillPhone 8 800 5659 6896 `
 -BillFax 545 45878 `
 -ShippFirstName John `
 -ShippLastName Smith `
 -ShippAddress1 Green str. 35 `
 -ShippAddress2 Green str. 35 `
 -ShippCity Chicago `
 -ShippPostcode 24545 `
 -ShippState IL `
 -ShippCountry US `
 -ShippCompany Apple `
 -ShippPhone 880086544564 `
 -ShippFax 556868 `
 -SubtotalPrice 563.23 `
 -TaxPrice 5.5 `
 -TotalPrice 23.56 `
 -TotalPaid 23.56 `
 -TotalWeight 23 `
 -PricesIncTax true `
 -ShippingPrice 5.5 `
 -ShippingTax 5.5 `
 -Discount 5.5 `
 -CouponDiscount 5.5 `
 -GiftCertificateDiscount 5.5 `
 -OrderShippingMethod UPS Ground `
 -CarrierId USPS `
 -WarehouseId 1 `
 -Coupons null `
 -Tags tag1,tag2 `
 -Comment This coole order `
 -AdminComment Test admin comment `
 -AdminPrivateComment Test admin private comment `
 -SendNotifications true `
 -SendAdminNotifications true `
 -ExternalSource POS `
 -InventoryBehaviour decrement_ignoring_policy `
 -CreateInvoice true `
 -NoteAttributes null `
 -ClearCache false `
 -Origin newsletter `
 -FeePrice 5.5 `
 -OrderItem null
```

- Convert the resource to JSON
```powershell
$OrderAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

