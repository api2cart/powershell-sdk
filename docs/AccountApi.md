# PSOpenAPITools.PSOpenAPITools\Api.AccountApi

All URIs are relative to *https://api.api2cart.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-AccountCartAdd**](AccountApi.md#Invoke-AccountCartAdd) | **POST** /account.cart.add.json | account.cart.add
[**Invoke-AccountCartList**](AccountApi.md#Invoke-AccountCartList) | **GET** /account.cart.list.json | account.cart.list
[**Invoke-AccountConfigUpdate**](AccountApi.md#Invoke-AccountConfigUpdate) | **PUT** /account.config.update.json | account.config.update
[**Invoke-AccountFailedWebhooks**](AccountApi.md#Invoke-AccountFailedWebhooks) | **GET** /account.failed_webhooks.json | account.failed_webhooks
[**Invoke-AccountSupportedPlatforms**](AccountApi.md#Invoke-AccountSupportedPlatforms) | **GET** /account.supported_platforms.json | account.supported_platforms


<a id="Invoke-AccountCartAdd"></a>
# **Invoke-AccountCartAdd**
> AccountCartAdd200Response Invoke-AccountCartAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AccountCartAdd] <PSCustomObject><br>

account.cart.add

Use this method to automate the process of connecting stores to API2Cart. The list of parameters will vary depending on the platform. To get a list of parameters that are specific to a particular shopping platform, you need to execute the account.supported_platforms.json method.

### Example
```powershell
# general setting of the PowerShell module, e.g. base URL, authentication, etc
$Configuration = Get-Configuration
# Configure API key authorization: ApiKeyAuth
$Configuration.ApiKey.x-api-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-api-key = "Bearer"

$AccountCartAddHybrisWebsitesInner = Initialize-AccountCartAddHybrisWebsitesInner -Uid "MyUid" -Url "MyUrl" -StoreIds "MyStoreIds"
$AccountCartAdd = Initialize-AccountCartAdd -CartId "3DCart" -StoreUrl "http://mystore.com" -BridgeUrl "https://your-store.com/custom/bridge/path/bridge.php" -StoreRoot "/home/www/stores/magento1922" -StoreKey "ab37fc230bc5df63a5be1b11220949be" -ValidateVersion $true -Verify $false -DbTablesPrefix "oc_" -UserAgent "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:47.0) Gecko/20100101 Firefox/47.0" -FtpHost "ftp.mystore.com" -FtpUser "user" -FtpPassword "G4}q215D4_H9$Be" -FtpPort 22 -FtpStoreDir "/public" -Var3dcartPrivateKey "7dba81f90bdbe25e7000e73214ca51b" -Var3dcartAccessToken "4Grr_ZCLNNoSUuhAjesKuchxo9SL" -Var3dcartapiApiKey "82cc921c6a5c67082cc921c6a5c6707e1d6e6862ba3201a" -AmazonSpClientId "amzn1.application-oa2-client.11e000e1f47d4998aca3733716d3b5a4" -AmazonSpClientSecret "2c987428209f235443221255bde064f4bdf8a65165a80f5d22760a83cb" -AmazonSpRefreshToken "Atzr|IwEBIPUI-bwRTdDgKNQ_g56C30wGqymtx30c9MdDC7Emwmojhs20k5BBG2hHtJiGZ_7OfG7khd1RuQr6KEst4qyWbo_eXi5S_T_VOxzJUuksG1cFOGFpFK-cnhReNzAeZIpZeJT7_ROy1csEFlQfC8FJS3bsbSkkbTz2ZcTN7_7ey0HVlhyfFizgROeSeOI24Wjs9l_KKzZW0jvi_oC2cxlIcyknnHLK6KMNz2rTXqQJWRtlK9xPJDdbcUa5STA8MQru91cxNBpSkZN_cq9OOELhbsIGKD75y7nZ3yJU4uHQC_9iBQQoFm0biKgi-kEQwOhwws8" -AmazonSpAwsRegion "us-east-1" -AmazonSpApiEnvironment "sandbox" -AmazonSellerId "13P636B2M1N4WR" -AspdotnetstorefrontApiUser "admin" -AspdotnetstorefrontApiPass "f6471ef78f72b41849a8b8b67791b0b5" -BigcommerceapiAdminAccount "admin" -BigcommerceapiApiPath "http://mystore.bigcommerce.com/api/v1" -BigcommerceapiApiKey "6b89704cd75738cb0f9f6468d5462aba" -BigcommerceapiClientId "p1r37bt131z86675nofv9xmhietoe4t" -BigcommerceapiAccessToken "igse8e4rdmzkxdi937qe69d59en1imw" -BigcommerceapiContext "stores/etplnf8o8v" -BolApiKey "51369628-feee-11ed-be56-0242ac120002" -BolApiSecret "8fGzEsbEP5z2MNZubmIil87m-sWzTkj?KDQKrmzmU!fA6aAUNMdKRp7LMWHwE!G37UMfnWByHBGSXJHkAG?QcuYTO2uklv4idIHwUMLHK!OO1yfRlWh!" -BolRetailerId 145001 -BigcartelUserName "subdomain" -BigcartelPassword "4GrrZCLNNoSUuhAjesKuchxo9SL" -DemandwareClientId "b849eb85-v8b9-1dw8-9fe2-97e1d6ffc7b0" -DemandwareApiPassword "testpassword" -DemandwareUserName "admin" -DemandwareUserPassword "12345" -EbayClientId "a9psel85v1wy5faeyjw03y0r" -EbayClientSecret "gmz3iz45x2" -EbayRuname "gmz3iz45x2" -EbayAccessToken "v^1.1#i ... AjRV4yNjA=" -EbayRefreshToken "v^1.1#i ... rAewqVasdA=" -EbayEnvironment "sandbox" -EbaySiteId 101 -WalmartClientId "423f6A24-123z-8654-989u-6fa96478289" -WalmartClientSecret "1gf85fea-8974-2648-w12w-rt54284tdf54" -WalmartEnvironment "production" -WalmartChannelType "0f3e4dd4-0514-4346-b39d-af0e00ea066d" -WalmartRegion "us" -EcwidAcessToken "igse8e4rdmzkxdi937qe69d59en1imw" -EcwidStoreId "1" -LazadaAppId "112577" -LazadaAppSecret "er33raICJ79Q5b0EsR9stmRnjE9XQ2WH" -LazadaRefreshToken "EAAPP06rM2n8BO4mZBuMPnu9zS0MaMbN7ue8aUkcxw4zewU337mVVb5br" -LazadaRegion "Malaysia" -LightspeedApiKey "cf5444729c2abd6b6a5d983691767cb5" -LightspeedApiSecret "2620ee52a8bc942f9d5d3a575f4d363e" -EtsyKeystring "a9psel85v1wy5faeyjw03y0r" -EtsySharedSecret "gmz3iz45x2" -EtsyAccessToken "igse8e4rdmzkxdi937qe69d59en1imw" -EtsyTokenSecret "igse8e4rdmzkxdi937qe69d59en1imw" -EtsyClientId "w0fi0igk2w29bjcd7ydr2s35" -EtsyRefreshToken "223577551.L07_RE-y7unmKf2dox4djsHkVxwpUfs1ikG_uQmHhF-aASEReNn_Qns1Wqn3dDa0ZMxrt9CIael3dgudeDZb31ZUdS" -FacebookAppId "6516912365277570" -FacebookAppSecret "737cf6bd2879cb6c7e5a8ff9cd63f3d46b0b5b7b" -FacebookAccessToken "EAAPP06rM2n8BO4mZBuMPnu9zS0MaMbN7ue8aUAhqbS58clzJwyp1rYRMpP31QJGziqtYbKypdVx3Cs0RpuufoUeLsbfX195XIB8VTlkcxw4zewU337mVVb5br" -FacebookBusinessId "294042786906655" -NetoApiKey "bbca57d8ff3c3677128112c15556d9e3" -NetoApiUsername "mylogin" -ShoplineAccessToken "igse8e4rdmzkxdi937qe69d59en1imw" -ShoplineAppKey "737cf6bd2879cb6c7e5a8ff9cd63f3d46b0b5b7b" -ShoplineAppSecret "1701d123bb5cc14cd2732dcaed90638316c0a09" -ShoplineSharedSecret "1701d123bb5cc14cd2732dcaed90638316c0a09" -ShopifyAccessToken "igse8e4rdmzkxdi937qe69d59en1imw" -ShopifyApiKey "bbca57d8ff3c3677128112c15556d9e3" -ShopifyApiPassword "860f3a6fc87632301a42cd88e4b5ab3d" -ShopifySharedSecret "gmz3iz45x2" -ShopeePartnerId "1276777" -ShopeePartnerKey "6a46494b4d746576554646626775617a577542774850636375464d6a736d5598" -ShopeeShopId "137968" -ShopeeRefreshToken "EAAPP06rM2n8BO4mZBuMPnu9zS0MaMbN7ue8aUkcxw4zewU987mVVb5br" -ShopeeRegion "CN" -ShopeeEnvironment "sandbox" -ShoplazzaAccessToken "igse8e4rdmzkxdi937qe69d59en1imw" -ShoplazzaSharedSecret "gmz3iz45x2" -ShopwareAccessKey "SWSCS3O1RJBSRNBYQLFIYJN2ZQ" -ShopwareApiKey "SWSCS3O1RJBSRNBYQLFIYJN2ZQ" -ShopwareApiSecret "V3NYNWg2b1dZdHBUWDN1cmdKdGhnenp5enVJYlJ0WlJvOFF2bnQ" -MivaAccessToken "227cbe434a1e358d72db0de993x9d9fd" -MivaSignature "1hpkrebfdsObGTor/0Gk9XcNBUQohrxrw67Sg9AM9ps=" -TiendanubeUserId 1234 -TiendanubeAccessToken "75bde7bb0b437475423e7e87c142c06052f80199" -TiendanubeClientSecret "5e3588f514a5ae0d0fa063d1b556531e25c83fa7e47472ed" -VolusionLogin "admin" -VolusionPassword "7943CA5F3990E00D9A4CCF0BD998211F" -HybrisClientId "api_client_1" -HybrisClientSecret "secret_phrase_1" -HybrisUsername "admin" -HybrisPassword "nimda" -HybrisWebsites $AccountCartAddHybrisWebsitesInner -SquareClientId "sq0idp-qwer_1pvuTYe9cAf1lmxyQ" -SquareClientSecret "c8d7077fce7b2b111111111898170695a01473a2ad" -SquareRefreshToken "EQAAlquVXMr6xIcPu7qPkIEAZ0thqChhQuowrvZIqOlwhOwhtmyh4ZRfesdRc434" -SquarespaceApiKey "8f7849d5-1411-47f2-9722-aa81c2a48d95" -SquarespaceClientId "9UGbUtS2V96BxRGmfOjsGAhTdsr9Vxxx" -SquarespaceClientSecret "GPZkUFkIKWg0KLE6rajsFMMYA9ma0udaaq2bYwBDXXX=" -SquarespaceAccessToken "SWSCS3O1RJBSRNBYQLFIYJN2ZQ" -SquarespaceRefreshToken "def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d" -CommercehqApiKey "sJrD-LM0eddhe63rfgfva0dDydXfre4" -CommercehqApiPassword "4Grr_ZCLNNoSUuhAjesKuchxo9SL" -WcConsumerKey "ck_26d8e2ad604f3917e429df6961722282bdcf109d" -WcConsumerSecret "cs_931ced666118a15c5f7b4a33a15gf5589cbeba55" -MagentoConsumerKey "ktv4n9rgrj0evjuy2t6p2xlb1f8u5pmy" -MagentoConsumerSecret "a46abc3kxyinlbggy06i9g975xqo6gjq" -MagentoAccessToken "igse8e4rdmzkxdi937qe69d59en1imw" -MagentoTokenSecret "igse8e4rdmzkxdi937qe69d59en1imw" -PrestashopWebserviceKey "CKJ1ZEWRJWRLTPVBQJ9FGGRORD4AGS96" -WixAppId "6b0b5b7b-7d87-45b5-bf34-ac6b438e63da" -WixAppSecretKey "316c0a09-f195-42be-74f6-a02cebb9cae6" -WixInstanceId "58b893a4-6b16-5c2f-qt78-qa3r61t32rt8" -WixRefreshToken "
        OAUTH2.eyJraWQiOiJkZ0x3cjNRMCIsImFsZyI6IkhTMjU2In0.
        eyJkYXRhIjoie1wiaWRcIjpcImJlZjM3MmRmLTUyNGItNDI3NS05M2RkL
        Tg4NDBlOTU3ZWU2OFwifSIsImlhdCI6MTY0ODA0NTEyNiwiZXhwIjoxNzExMTE3MTI2fQ.
        VRR2lGSbcTVmaArtmyyhy6o4WRDwTn-nlDCQpZ97eYw
      " -MercadoLibreAppId "211188015100135" -MercadoLibreAppSecretKey "e2qoG2zklLlfP7cEngEJ94YjhkejkjAm" -MercadoLibreRefreshToken "TG-63h13529vb5464110188d2x9-703754376" -ZidClientId 1234 -ZidClientSecret "nl5l1lE0vxgv6cV111fHsdlOOIfb0Ms5IR7l4Igs" -ZidAccessToken "def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d" -ZidAuthorization "def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d" -ZidRefreshToken "def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d" -FlipkartClientId "19414773883a13a850b6a52350b7246499a24" -FlipkartClientSecret "nl5l1lE0vxgv6cV111fHsdlOOIfb0Ms5IR7l4Igs" -AllegroClientId "2915e189ce3d23d23d2327d204ae6a0bd" -AllegroClientSecret "DNHtqdL2WPIefeUhQWYgtXPS23fgbfgasdsGHHJGhg3RTFDQWFGZmVoFRT5IfkQj1E7eR5" -AllegroAccessToken "eyJhbGciOiJSUzI1NiIsInR5cCI6IsfddfdfdeyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI" -AllegroRefreshToken "eyJhbGciOiJSUzI1NiIsInR5cCI6IsfddfdfdeyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI" -AllegroEnvironment "sandbox" -ZohoClientId "1000.FLCHGI2LS1111111TOR4OGB697W4IX" -ZohoClientSecret "c8d7077fce7b2b111111111898170695a01473a2ad" -ZohoRefreshToken "1000.11111111111111111111111111111111.1b3ca6f054341a111118abf928beb33b" -ZohoRegion "Europe" -OttoClientId "911a3dbf-d261-4763-cc81-052876465b55" -OttoClientSecret "9887a82a-2879-421e-a6wc-54e986b3458c" -OttoAppId "6eaef6a3-822e-425b-8mc9-53750063e34d" -OttoRefreshToken "eyJhbGciOiJSUzI1NiIsInR5cCI6IsfddfdfdeyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI" -OttoEnvironment "sandbox" -OttoAccessToken "eyJhbGciOiJS34535f45f54f5656deyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI" -TiktokshopAppKey "6arbhkzno8nbv" -TiktokshopAppSecret "d95820a05a0cd54fb394fcd26fgat63999b183bc" -TiktokshopRefreshToken "TTP_NTUxZTNhYTQ2ZDk2YmRmZWNmYWY2YWY12345NGYwNjQ3YjkzYTllYjA0YmNlMw" -TiktokshopAccessToken "TTP_Fw8r12345kW03FYd09DG-9INtpw361hWthei12345iPJ5AUv99fLSCYD9-Uu12345TgNRzKZxi5-tfFMtdWqglEt5_iCk" -SallaClientId "1bxxxcf9-5xx4-xxx-bxxf-929b8xxxxe11" -SallaClientSecret "8x88axxxc25e1fxxxa1c06fxxx150xx5" -SallaRefreshToken "oxy_rt_zxxxxiY2xxZWWxxxxlU-tROxxxxx2JzS2fwzxxxxxkU.p3xxxkCIyFexxxxP50WwZYfhw5_wg1xxxxV5F-8xxXc" -SallaAccessToken "oxy_rt_zxxxxiY2xxZWWxxxxlU-tROxxxxx2JzS2fwzxxxxxkU.p3xxxkCIyFexxxxP50WwZYfhw5_wg1xxxxV5F-8xxXc" -TemuAppKey "4ebbc9190ae410443d65b4c2faca9811" -TemuAppSecret "4782d2d827276688bf4758bed55dbdd4bbe79a78" -TemuAccessToken "uplv3hfyt5kcwoymrgnajnbl1ow5qxlz4sqhev6hl3xosz5dejrtyl2jre6" -TemuRegion "US" # AccountCartAdd | 

# account.cart.add
try {
    $Result = Invoke-AccountCartAdd -AccountCartAdd $AccountCartAdd
} catch {
    Write-Host ("Exception occurred when calling Invoke-AccountCartAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **AccountCartAdd** | [**AccountCartAdd**](AccountCartAdd.md)|  | 

### Return type

[**AccountCartAdd200Response**](AccountCartAdd200Response.md) (PSCustomObject)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AccountCartList"></a>
# **Invoke-AccountCartList**
> AccountCartList200Response Invoke-AccountCartList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreUrl] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-RequestFromDate] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-RequestToDate] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

account.cart.list

This method lets you get a list of online stores connected to your API2Cart account. You can get the number of API requests to each store if you specify a period using parameters (request_from_date, request_to_date). The total_calls field is displayed only if there are parameters (request_from_date, request_to_date).

### Example
```powershell
# general setting of the PowerShell module, e.g. base URL, authentication, etc
$Configuration = Get-Configuration
# Configure API key authorization: ApiKeyAuth
$Configuration.ApiKey.x-api-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-api-key = "Bearer"

$StoreUrl = "http://mystore.com" # String | A web address of a store (optional)
$StoreKey = "ab37fc230bc5df63a5be1b11220949be" # String | Find store by store key (optional)
$RequestFromDate = "2010-07-29" # String | Retrieve entities from their creation date (optional)
$RequestToDate = "2100-08-29" # String | Retrieve entities to their creation date (optional)
$Params = "url,store_key" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "force_all")
$Exclude = "url,store_key" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# account.cart.list
try {
    $Result = Invoke-AccountCartList -StoreUrl $StoreUrl -StoreKey $StoreKey -RequestFromDate $RequestFromDate -RequestToDate $RequestToDate -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-AccountCartList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **StoreUrl** | **String**| A web address of a store | [optional] 
 **StoreKey** | **String**| Find store by store key | [optional] 
 **RequestFromDate** | **String**| Retrieve entities from their creation date | [optional] 
 **RequestToDate** | **String**| Retrieve entities to their creation date | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;force_all&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**AccountCartList200Response**](AccountCartList200Response.md) (PSCustomObject)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AccountConfigUpdate"></a>
# **Invoke-AccountConfigUpdate**
> AccountConfigUpdate200Response Invoke-AccountConfigUpdate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ReplaceParameters] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-NewStoreUrl] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-NewStoreKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BridgeUrl] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreRoot] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DbTablesPrefix] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-UserAgent] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Var3dcartPrivateKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Var3dcartAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Var3dcartapiApiKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AmazonSpClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AmazonSpClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AmazonSpRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AmazonSpAwsRegion] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AmazonSpApiEnvironment] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AmazonSellerId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AspdotnetstorefrontApiUser] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AspdotnetstorefrontApiPass] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BigcommerceapiAdminAccount] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BigcommerceapiApiPath] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BigcommerceapiApiKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BigcommerceapiClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BigcommerceapiAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BigcommerceapiContext] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BolApiKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BolApiSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BolRetailerId] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DemandwareClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DemandwareApiPassword] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DemandwareUserName] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DemandwareUserPassword] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EbayClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EbayClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EbayRuname] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EbayAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EbayRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EbayEnvironment] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EbaySiteId] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EcwidAcessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EcwidStoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LazadaAppId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LazadaAppSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LazadaRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LazadaRegion] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EtsyKeystring] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EtsySharedSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EtsyAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EtsyTokenSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EtsyClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EtsyRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FacebookAppId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FacebookAppSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FacebookAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FacebookBusinessId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-NetoApiKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-NetoApiUsername] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShoplineAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShoplineAppKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShoplineAppSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShoplineSharedSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopifyAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopifyApiKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopifyApiPassword] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopifySharedSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopeePartnerId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopeePartnerKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopeeShopId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopeeRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopeeRegion] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopeeEnvironment] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShoplazzaAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShoplazzaSharedSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MivaAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MivaSignature] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopwareAccessKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopwareApiKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShopwareApiSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BigcartelUserName] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BigcartelPassword] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-VolusionLogin] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-VolusionPassword] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-WalmartClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-WalmartClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-WalmartEnvironment] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-WalmartChannelType] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-WalmartRegion] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SquareClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SquareClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SquareRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SquarespaceApiKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SquarespaceClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SquarespaceClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SquarespaceAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SquarespaceRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-HybrisClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-HybrisClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-HybrisUsername] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-HybrisPassword] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-HybrisWebsites] <String[]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LightspeedApiKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LightspeedApiSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CommercehqApiKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CommercehqApiPassword] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-WcConsumerKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-WcConsumerSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MagentoConsumerKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MagentoConsumerSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MagentoAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MagentoTokenSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PrestashopWebserviceKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-WixAppId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-WixAppSecretKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-WixInstanceId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-WixRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MercadoLibreAppId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MercadoLibreAppSecretKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MercadoLibreRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ZidClientId] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ZidClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ZidAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ZidAuthorization] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ZidRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FlipkartClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FlipkartClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AllegroClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AllegroClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AllegroAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AllegroRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AllegroEnvironment] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ZohoClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ZohoClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ZohoRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ZohoRegion] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-TiendanubeUserId] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-TiendanubeAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-TiendanubeClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OttoClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OttoClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OttoAppId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OttoRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OttoEnvironment] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OttoAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-TiktokshopAppKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-TiktokshopAppSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-TiktokshopRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-TiktokshopAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SallaClientId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SallaClientSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SallaRefreshToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SallaAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-TemuAppKey] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-TemuAppSecret] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-TemuAccessToken] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-TemuRegion] <String><br>

account.config.update

Use this method to automate the change of credentials used to connect online stores. The list of supported parameters differs depending on the platform.

### Example
```powershell
# general setting of the PowerShell module, e.g. base URL, authentication, etc
$Configuration = Get-Configuration
# Configure API key authorization: StoreKeyAuth
$Configuration.ApiKey.x-store-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-store-key = "Bearer"

# Configure API key authorization: ApiKeyAuth
$Configuration.ApiKey.x-api-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-api-key = "Bearer"

$ReplaceParameters = $true # Boolean | Identifies if there is a necessity to replace parameters (optional)
$NewStoreUrl = "http://mystore.com" # String | The web address of the store you want to update to connect to API2Cart (optional)
$NewStoreKey = "b636495648de3086f6f57b1bd4be548f" # String | Update store key (optional)
$BridgeUrl = "https://your-store.com/custom/bridge/path/bridge.php" # String | This parameter allows to set up store with custom bridge url (also you must use store_root parameter if a bridge folder is not in the root folder of the store) (optional)
$StoreRoot = "/home/www/stores/magento1922" # String | Absolute path to the store root directory (used with ""bridge_url"" parameter) (optional)
$DbTablesPrefix = "oc_" # String | DB tables prefix (optional)
$UserAgent = "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:47.0) Gecko/20100101 Firefox/47.0" # String | This parameter allows you to set your custom user agent, which will be used in requests to the store. Please use it cautiously, as the store's firewall may block specific values. (optional)
$Var3dcartPrivateKey = "7dba81f90bdbe25e7000e73214ca51b" # String | 3DCart Private Key (optional)
$Var3dcartAccessToken = "4Grr_ZCLNNoSUuhAjesKuchxo9SL" # String | 3DCart Token (optional)
$Var3dcartapiApiKey = "82cc921c6a5c67082cc921c6a5c6707e1d6e6862ba3201a" # String | 3DCart API Key (optional)
$AmazonSpClientId = "amzn1.application-oa2-client.11e000e1f47d4998aca3733716d3b5a4" # String | Amazon SP API app client id (optional)
$AmazonSpClientSecret = "2c987428209f235443221255bde064f4bdf8a65165a80f5d22760a83cb" # String | Amazon SP API app client secret (optional)
$AmazonSpRefreshToken = "Atzr|IwEBIPUI-bwRTdDgKNQ_g56C30wGqymtx30c9MdDC7Emwmojhs20k5BBG2hHtJiGZ_7OfG7khd1RuQr6KEst4qyWbo_eXi5S_T_VOxzJUuksG1cFOGFpFK-cnhReNzAeZIpZeJT7_ROy1csEFlQfC8FJS3bsbSkkbTz2ZcTN7_7ey0HVlhyfFizgROeSeOI24Wjs9l_KKzZW0jvi_oC2cxlIcyknnHLK6KMNz2rTXqQJWRtlK9xPJDdbcUa5STA8MQru91cxNBpSkZN_cq9OOELhbsIGKD75y7nZ3yJU4uHQC_9iBQQoFm0biKgi-kEQwOhwws8" # String | Amazon SP API OAuth refresh token (optional)
$AmazonSpAwsRegion = "us-east-1" # String | Amazon AWS Region (optional)
$AmazonSpApiEnvironment = "sandbox" # String | Amazon SP API environment (optional) (default to "production")
$AmazonSellerId = "13P636B2M1N4WR" # String | Amazon Seller ID (Merchant token) (optional)
$AspdotnetstorefrontApiUser = "admin" # String | It's a AspDotNetStorefront account for which API is available (optional)
$AspdotnetstorefrontApiPass = "f6471ef78f72b41849a8b8b67791b0b5" # String | AspDotNetStorefront API Password (optional)
$BigcommerceapiAdminAccount = "admin" # String | It's a BigCommerce account for which API is enabled (optional)
$BigcommerceapiApiPath = "http://mystore.bigcommerce.com/api/v1" # String | BigCommerce API URL (optional)
$BigcommerceapiApiKey = "6b89704cd75738cb0f9f6468d5462aba" # String | Bigcommerce API Key (optional)
$BigcommerceapiClientId = "p1r37bt131z86675nofv9xmhietoe4t" # String | Client ID of the requesting app (optional)
$BigcommerceapiAccessToken = "igse8e4rdmzkxdi937qe69d59en1imw" # String | Access token authorizing the app to access resources on behalf of a user (optional)
$BigcommerceapiContext = "stores/etplnf8o8v" # String | API Path section unique to the store (optional)
$BolApiKey = "51369628-feee-11ed-be56-0242ac120002" # String | Bol API Key (optional)
$BolApiSecret = "8fGzEsbEP5z2MNZubmIil87m-sWzTkj?KDQKrmzmU!fA6aAUNMdKRp7LMWHwE!G37UMfnWByHBGSXJHkAG?QcuYTO2uklv4idIHwUMLHK!OO1yfRlWh!" # String | Bol API Secret (optional)
$BolRetailerId = 145001 # Int32 | Bol Retailer ID (optional)
$DemandwareClientId = "b849eb85-v8b9-1dw8-9fe2-97e1d6ffc7b0" # String | Demandware client id (optional)
$DemandwareApiPassword = "testpassword" # String | Demandware api password (optional)
$DemandwareUserName = "admin" # String | Demandware user name (optional)
$DemandwareUserPassword = "12345" # String | Demandware user password (optional)
$EbayClientId = "a9psel85v1wy5faeyjw03y0r" # String | Application ID (AppID). (optional)
$EbayClientSecret = "gmz3iz45x2" # String | Shared Secret from eBay application (optional)
$EbayRuname = "gmz3iz45x2" # String | The RuName value that eBay assigns to your application. (optional)
$EbayAccessToken = "v^1.1#i ... AjRV4yNjA=" # String | Used to authenticate API requests. (optional)
$EbayRefreshToken = "v^1.1#i ... rAewqVasdA=" # String | Used to renew the access token. (optional)
$EbayEnvironment = "sandbox" # String | eBay environment (optional)
$EbaySiteId = 101 # Int32 | eBay global ID (optional) (default to 0)
$EcwidAcessToken = "igse8e4rdmzkxdi937qe69d59en1imw" # String | Access token authorizing the app to access resources on behalf of a user (optional)
$EcwidStoreId = "1" # String | Store Id (optional)
$LazadaAppId = "112577" # String | Lazada App ID (optional)
$LazadaAppSecret = "er33raICJ79Q5b0EsR9stmRnjE9XQ2WH" # String | Lazada App Secret (optional)
$LazadaRefreshToken = "EAAPP06rM2n8BO4mZBuMPnu9zS0MaMbN7ue8aUkcxw4zewU337mVVb5br" # String | Lazada Refresh Token (optional)
$LazadaRegion = "Malaysia" # String | Lazada API endpoint Region (optional)
$EtsyKeystring = "a9psel85v1wy5faeyjw03y0r" # String | Etsy keystring (optional)
$EtsySharedSecret = "gmz3iz45x2" # String | Etsy shared secret (optional)
$EtsyAccessToken = "igse8e4rdmzkxdi937qe69d59en1imw" # String | Access token authorizing the app to access resources on behalf of a user (optional)
$EtsyTokenSecret = "igse8e4rdmzkxdi937qe69d59en1imw" # String | Secret token authorizing the app to access resources on behalf of a user (optional)
$EtsyClientId = "w0fi0igk2w29bjcd7ydr2s35" # String | Etsy Client Id (optional)
$EtsyRefreshToken = "223577551.L07_RE-y7unmKf2dox4djsHkVxwpUfs1ikG_uQmHhF-aASEReNn_Qns1Wqn3dDa0ZMxrt9CIael3dgudeDZb31ZUdS" # String | Etsy Refresh token (optional)
$FacebookAppId = "6516912365277570" # String | Facebook App ID (optional)
$FacebookAppSecret = "737cf6bd2879cb6c7e5a8ff9cd63f3d46b0b5b7b" # String | Facebook App Secret (optional)
$FacebookAccessToken = "EAAPP06rM2n8BO4mZBuMPnu9zS0MaMbN7ue8aUAhqbS58clzJwyp1rYRMpP31QJGziqtYbKypdVx3Cs0RpuufoUeLsbfX195XIB8VTlkcxw4zewU337mVVb5br" # String | Facebook Access Token (optional)
$FacebookBusinessId = "294042786906655" # String | Facebook Business ID (optional)
$NetoApiKey = "bbca57d8ff3c3677128112c15556d9e3" # String | Neto API Key (optional)
$NetoApiUsername = "mylogin" # String | Neto User Name (optional)
$ShoplineAccessToken = "igse8e4rdmzkxdi937qe69d59en1imw" # String | Shopline APP Key (optional)
$ShoplineAppKey = "737cf6bd2879cb6c7e5a8ff9cd63f3d46b0b5b7b" # String | Shopline APP Key (optional)
$ShoplineAppSecret = "1701d123bb5cc14cd2732dcaed90638316c0a09" # String | Shopline App Secret (optional)
$ShoplineSharedSecret = "1701d123bb5cc14cd2732dcaed90638316c0a09" # String | Shopline Shared Secret (optional)
$ShopifyAccessToken = "igse8e4rdmzkxdi937qe69d59en1imw" # String | Access token authorizing the app to access resources on behalf of a user (optional)
$ShopifyApiKey = "bbca57d8ff3c3677128112c15556d9e3" # String | Shopify API Key (optional)
$ShopifyApiPassword = "860f3a6fc87632301a42cd88e4b5ab3d" # String | Shopify API Password (optional)
$ShopifySharedSecret = "gmz3iz45x2" # String | Shared secret (optional)
$ShopeePartnerId = "1276777" # String | Shopee Partner ID (optional)
$ShopeePartnerKey = "6a46494b4d746576554646626775617a577542774850636375464d6a736d5598" # String | Shopee Partner Key (optional)
$ShopeeShopId = "137968" # String | Shopee SHOP ID (optional)
$ShopeeRefreshToken = "EAAPP06rM2n8BO4mZBuMPnu9zS0MaMbN7ue8aUkcxw4zewU987mVVb5br" # String | Shopee Refresh Token (optional)
$ShopeeRegion = "CN" # String | Shopee API endpoint Region. Use for Chinese Mainland or Brazil. (optional)
$ShopeeEnvironment = "sandbox" # String | Shopee Environment (optional)
$ShoplazzaAccessToken = "igse8e4rdmzkxdi937qe69d59en1imw" # String | Access token authorizing the app to access resources on behalf of a user (optional)
$ShoplazzaSharedSecret = "gmz3iz45x2" # String | Shared secret (optional)
$MivaAccessToken = "227cbe434a1e358d72db0de993x9d9fd" # String | Miva access token (optional)
$MivaSignature = "1hpkrebfdsObGTor/0Gk9XcNBUQohrxrw67Sg9AM9ps=" # String | Miva signature (optional)
$ShopwareAccessKey = "SWSCS3O1RJBSRNBYQLFIYJN2ZQ" # String | Shopware access key (optional)
$ShopwareApiKey = "SWSCS3O1RJBSRNBYQLFIYJN2ZQ" # String | Shopware api key (optional)
$ShopwareApiSecret = "V3NYNWg2b1dZdHBUWDN1cmdKdGhnenp5enVJYlJ0WlJvOFF2bnQ" # String | Shopware client secret access key (optional)
$BigcartelUserName = "subdomain" # String | Subdomain of store (optional)
$BigcartelPassword = "4GrrZCLNNoSUuhAjesKuchxo9SL" # String | BigCartel account password (optional)
$VolusionLogin = "admin" # String | It's a Volusion account for which API is enabled (optional)
$VolusionPassword = "7943CA5F3990E00D9A4CCF0BD998211F" # String | Volusion API Password (optional)
$WalmartClientId = "423f6A24-123z-8654-989u-6fa96478289" # String | Walmart client ID. For the region 'ca' use Consumer ID (optional)
$WalmartClientSecret = "1gf85fea-8974-2648-w12w-rt54284tdf54" # String | Walmart client secret. For the region 'ca' use Private Key (optional)
$WalmartEnvironment = "production" # String | Walmart environment (optional) (default to "production")
$WalmartChannelType = "0f3e4dd4-0514-4346-b39d-af0e00ea066d" # String | Walmart WM_CONSUMER.CHANNEL.TYPE header (optional)
$WalmartRegion = "us" # String | Walmart region (optional) (default to "us")
$SquareClientId = "sq0idp-qwer_1pvuTYe9cAf1lmxyQ" # String | Square (Weebly) Client ID (optional)
$SquareClientSecret = "c8d7077fce7b2b111111111898170695a01473a2ad" # String | Square (Weebly) Client Secret (optional)
$SquareRefreshToken = "EQAAlquVXMr6xIcPu7qPkIEAZ0thqChhQuowrvZIqOlwhOwhtmyh4ZRfesdRc434" # String | Square (Weebly) Refresh Token (optional)
$SquarespaceApiKey = "8f7849d5-1411-47f2-9722-aa81c2a48d95" # String | Squarespace API Key (optional)
$SquarespaceClientId = "9UGbUtS2V96BxRGmfOjsGAhTdsr9Vxxx" # String | Squarespace Connector Client ID (optional)
$SquarespaceClientSecret = "GPZkUFkIKWg0KLE6rajsFMMYA9ma0udaaq2bYwBDXXX=" # String | Squarespace Connector Client Secret (optional)
$SquarespaceAccessToken = "SWSCS3O1RJBSRNBYQLFIYJN2ZQ" # String | Squarespace access token (optional)
$SquarespaceRefreshToken = "def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d" # String | Squarespace refresh token (optional)
$HybrisClientId = "api_client_1" # String | Omni Commerce Connector Client ID (optional)
$HybrisClientSecret = "secret_phrase_1" # String | Omni Commerce Connector Client Secret (optional)
$HybrisUsername = "admin" # String | User Name (optional)
$HybrisPassword = "nimda" # String | User password (optional)
$HybrisWebsites = "MyHybrisWebsites" # String[] | Websites to stores mapping data (optional)
$LightspeedApiKey = "cf5444729c2abd6b6a5d983691767cb5" # String | LightSpeed api key (optional)
$LightspeedApiSecret = "2620ee52a8bc942f9d5d3a575f4d363e" # String | LightSpeed api secret (optional)
$CommercehqApiKey = "sJrD-LM0eddhe63rfgfva0dDydXfre4" # String | CommerceHQ api key (optional)
$CommercehqApiPassword = "4Grr_ZCLNNoSUuhAjesKuchxo9SL" # String | CommerceHQ api password (optional)
$WcConsumerKey = "ck_26d8e2ad604f3917e429df6961722282bdcf109d" # String | Woocommerce consumer key (optional)
$WcConsumerSecret = "cs_931ced666118a15c5f7b4a33a15gf5589cbeba55" # String | Woocommerce consumer secret (optional)
$MagentoConsumerKey = "ktv4n9rgrj0evjuy2t6p2xlb1f8u5pmy" # String | Magento Consumer Key (optional)
$MagentoConsumerSecret = "a46abc3kxyinlbggy06i9g975xqo6gjq" # String | Magento Consumer Secret (optional)
$MagentoAccessToken = "igse8e4rdmzkxdi937qe69d59en1imw" # String | Magento Access Token (optional)
$MagentoTokenSecret = "igse8e4rdmzkxdi937qe69d59en1imw" # String | Magento Token Secret (optional)
$PrestashopWebserviceKey = "CKJ1ZEWRJWRLTPVBQJ9FGGRORD4AGS96" # String | Prestashop webservice key (optional)
$WixAppId = "6b0b5b7b-7d87-45b5-bf34-ac6b438e63da" # String | Wix App ID (optional)
$WixAppSecretKey = "316c0a09-f195-42be-74f6-a02cebb9cae6" # String | Wix App Secret Key (optional)
$WixInstanceId = "58b893a4-6b16-5c2f-qt78-qa3r61t32rt8" # String | Wix Instance ID (optional)
$WixRefreshToken = "
        OAUTH2.eyJraWQiOiJkZ0x3cjNRMCIsImFsZyI6IkhTMjU2In0.
        eyJkYXRhIjoie1wiaWRcIjpcImJlZjM3MmRmLTUyNGItNDI3NS05M2RkL
        Tg4NDBlOTU3ZWU2OFwifSIsImlhdCI6MTY0ODA0NTEyNiwiZXhwIjoxNzExMTE3MTI2fQ.
        VRR2lGSbcTVmaArtmyyhy6o4WRDwTn-nlDCQpZ97eYw
      " # String | Wix refresh token (optional)
$MercadoLibreAppId = "211188015100135" # String | Mercado Libre App ID (optional)
$MercadoLibreAppSecretKey = "e2qoG2zklLlfP7cEngEJ94YjhkejkjAm" # String | Mercado Libre App Secret Key (optional)
$MercadoLibreRefreshToken = "TG-63h13529vb5464110188d2x9-703754376" # String | Mercado Libre Refresh Token (optional)
$ZidClientId = 1234 # Int32 | Zid Client ID (optional)
$ZidClientSecret = "nl5l1lE0vxgv6cV111fHsdlOOIfb0Ms5IR7l4Igs" # String | Zid Client Secret (optional)
$ZidAccessToken = "def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d" # String | Zid Access Token (optional)
$ZidAuthorization = "def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d" # String | Zid Authorization (optional)
$ZidRefreshToken = "def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d" # String | Zid refresh token (optional)
$FlipkartClientId = "19414773883a13a850b6a52350b7246499a24" # String | Flipkart Client ID (optional)
$FlipkartClientSecret = "nl5l1lE0vxgv6cV111fHsdlOOIfb0Ms5IR7l4Igs" # String | Flipkart Client Secret (optional)
$AllegroClientId = "2915e189ce3d23d23d2327d204ae6a0bd" # String | Allegro Client ID (optional)
$AllegroClientSecret = "DNHtqdL2WPIefeUhQWYgtXPS23fgbfgasdsGHHJGhg3RTFDQWFGZmVoFRT5IfkQj1E7eR5" # String | Allegro Client Secret (optional)
$AllegroAccessToken = "eyJhbGciOiJSUzI1NiIsInR5cCI6IsfddfdfdeyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI" # String | Allegro Access Token (optional)
$AllegroRefreshToken = "eyJhbGciOiJSUzI1NiIsInR5cCI6IsfddfdfdeyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI" # String | Allegro Refresh Token (optional)
$AllegroEnvironment = "sandbox" # String | Allegro Environment (optional) (default to "production")
$ZohoClientId = "1000.FLCHGI2LS1111111TOR4OGB697W4IX" # String | Zoho Client ID (optional)
$ZohoClientSecret = "c8d7077fce7b2b111111111898170695a01473a2ad" # String | Zoho Client Secret (optional)
$ZohoRefreshToken = "1000.11111111111111111111111111111111.1b3ca6f054341a111118abf928beb33b" # String | Zoho Refresh Token (optional)
$ZohoRegion = "Europe" # String | Zoho API endpoint Region (optional)
$TiendanubeUserId = 1234 # Int32 | Tiendanube User ID (optional)
$TiendanubeAccessToken = "75bde7bb0b437475423e7e87c142c06052f80199" # String | Tiendanube Access Token (optional)
$TiendanubeClientSecret = "5e3588f514a5ae0d0fa063d1b556531e25c83fa7e47472ed" # String | Tiendanube Client Secret (optional)
$OttoClientId = "911a3dbf-d261-4763-cc81-052876465b55" # String | Otto Client ID (optional)
$OttoClientSecret = "9887a82a-2879-421e-a6wc-54e986b3458c" # String | Otto Client Secret (optional)
$OttoAppId = "6eaef6a3-822e-425b-8mc9-53750063e34d" # String | Otto App ID (optional)
$OttoRefreshToken = "eyJhbGciOiJSUzI1NiIsInR5cCI6IsfddfdfdeyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI" # String | Otto Refresh Token (optional)
$OttoEnvironment = "sandbox" # String | Otto Environment (optional)
$OttoAccessToken = "eyJhbGciOiJS34535f45f54f5656deyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI" # String | Otto Access Token (optional)
$TiktokshopAppKey = "6arbhkzno8nbv" # String | TikTok Shop App Key (optional)
$TiktokshopAppSecret = "d95820a05a0cd54fb394fcd26fgat63999b183bc" # String | TikTok Shop App Secret (optional)
$TiktokshopRefreshToken = "TTP_NTUxZTNhYTQ2ZDk2YmRmZWNmYWY2YWY12345NGYwNjQ3YjkzYTllYjA0YmNlMw" # String | TikTok Shop Refresh Token (optional)
$TiktokshopAccessToken = "TTP_Fw8r12345kW03FYd09DG-9INtpw361hWthei12345iPJ5AUv99fLSCYD9-Uu12345TgNRzKZxi5-tfFMtdWqglEt5_iCk" # String | TikTok Shop Access Token (optional)
$SallaClientId = "1bxxxcf9-5xx4-xxx-bxxf-929b8xxxxe11" # String | Salla Client ID (optional)
$SallaClientSecret = "8x88axxxc25e1fxxxa1c06fxxx150xx5" # String | Salla Client Secret (optional)
$SallaRefreshToken = "oxy_rt_zxxxxiY2xxZWWxxxxlU-tROxxxxx2JzS2fwzxxxxxkU.p3xxxkCIyFexxxxP50WwZYfhw5_wg1xxxxV5F-8xxXc" # String | Salla Refresh Token (optional)
$SallaAccessToken = "oxy_rt_zxxxxiY2xxZWWxxxxlU-tROxxxxx2JzS2fwzxxxxxkU.p3xxxkCIyFexxxxP50WwZYfhw5_wg1xxxxV5F-8xxXc" # String | Salla Access Token (optional)
$TemuAppKey = "4ebbc9190ae410443d65b4c2faca9811" # String | Temu App Key (optional)
$TemuAppSecret = "4782d2d827276688bf4758bed55dbdd4bbe79a78" # String | Temu App Secret (optional)
$TemuAccessToken = "uplv3hfyt5kcwoymrgnajnbl1ow5qxlz4sqhev6hl3xosz5dejrtyl2jre6" # String | Temu Access Token (optional)
$TemuRegion = "US" # String | Temu API endpoint Region. (optional)

# account.config.update
try {
    $Result = Invoke-AccountConfigUpdate -ReplaceParameters $ReplaceParameters -NewStoreUrl $NewStoreUrl -NewStoreKey $NewStoreKey -BridgeUrl $BridgeUrl -StoreRoot $StoreRoot -DbTablesPrefix $DbTablesPrefix -UserAgent $UserAgent -Var3dcartPrivateKey $Var3dcartPrivateKey -Var3dcartAccessToken $Var3dcartAccessToken -Var3dcartapiApiKey $Var3dcartapiApiKey -AmazonSpClientId $AmazonSpClientId -AmazonSpClientSecret $AmazonSpClientSecret -AmazonSpRefreshToken $AmazonSpRefreshToken -AmazonSpAwsRegion $AmazonSpAwsRegion -AmazonSpApiEnvironment $AmazonSpApiEnvironment -AmazonSellerId $AmazonSellerId -AspdotnetstorefrontApiUser $AspdotnetstorefrontApiUser -AspdotnetstorefrontApiPass $AspdotnetstorefrontApiPass -BigcommerceapiAdminAccount $BigcommerceapiAdminAccount -BigcommerceapiApiPath $BigcommerceapiApiPath -BigcommerceapiApiKey $BigcommerceapiApiKey -BigcommerceapiClientId $BigcommerceapiClientId -BigcommerceapiAccessToken $BigcommerceapiAccessToken -BigcommerceapiContext $BigcommerceapiContext -BolApiKey $BolApiKey -BolApiSecret $BolApiSecret -BolRetailerId $BolRetailerId -DemandwareClientId $DemandwareClientId -DemandwareApiPassword $DemandwareApiPassword -DemandwareUserName $DemandwareUserName -DemandwareUserPassword $DemandwareUserPassword -EbayClientId $EbayClientId -EbayClientSecret $EbayClientSecret -EbayRuname $EbayRuname -EbayAccessToken $EbayAccessToken -EbayRefreshToken $EbayRefreshToken -EbayEnvironment $EbayEnvironment -EbaySiteId $EbaySiteId -EcwidAcessToken $EcwidAcessToken -EcwidStoreId $EcwidStoreId -LazadaAppId $LazadaAppId -LazadaAppSecret $LazadaAppSecret -LazadaRefreshToken $LazadaRefreshToken -LazadaRegion $LazadaRegion -EtsyKeystring $EtsyKeystring -EtsySharedSecret $EtsySharedSecret -EtsyAccessToken $EtsyAccessToken -EtsyTokenSecret $EtsyTokenSecret -EtsyClientId $EtsyClientId -EtsyRefreshToken $EtsyRefreshToken -FacebookAppId $FacebookAppId -FacebookAppSecret $FacebookAppSecret -FacebookAccessToken $FacebookAccessToken -FacebookBusinessId $FacebookBusinessId -NetoApiKey $NetoApiKey -NetoApiUsername $NetoApiUsername -ShoplineAccessToken $ShoplineAccessToken -ShoplineAppKey $ShoplineAppKey -ShoplineAppSecret $ShoplineAppSecret -ShoplineSharedSecret $ShoplineSharedSecret -ShopifyAccessToken $ShopifyAccessToken -ShopifyApiKey $ShopifyApiKey -ShopifyApiPassword $ShopifyApiPassword -ShopifySharedSecret $ShopifySharedSecret -ShopeePartnerId $ShopeePartnerId -ShopeePartnerKey $ShopeePartnerKey -ShopeeShopId $ShopeeShopId -ShopeeRefreshToken $ShopeeRefreshToken -ShopeeRegion $ShopeeRegion -ShopeeEnvironment $ShopeeEnvironment -ShoplazzaAccessToken $ShoplazzaAccessToken -ShoplazzaSharedSecret $ShoplazzaSharedSecret -MivaAccessToken $MivaAccessToken -MivaSignature $MivaSignature -ShopwareAccessKey $ShopwareAccessKey -ShopwareApiKey $ShopwareApiKey -ShopwareApiSecret $ShopwareApiSecret -BigcartelUserName $BigcartelUserName -BigcartelPassword $BigcartelPassword -VolusionLogin $VolusionLogin -VolusionPassword $VolusionPassword -WalmartClientId $WalmartClientId -WalmartClientSecret $WalmartClientSecret -WalmartEnvironment $WalmartEnvironment -WalmartChannelType $WalmartChannelType -WalmartRegion $WalmartRegion -SquareClientId $SquareClientId -SquareClientSecret $SquareClientSecret -SquareRefreshToken $SquareRefreshToken -SquarespaceApiKey $SquarespaceApiKey -SquarespaceClientId $SquarespaceClientId -SquarespaceClientSecret $SquarespaceClientSecret -SquarespaceAccessToken $SquarespaceAccessToken -SquarespaceRefreshToken $SquarespaceRefreshToken -HybrisClientId $HybrisClientId -HybrisClientSecret $HybrisClientSecret -HybrisUsername $HybrisUsername -HybrisPassword $HybrisPassword -HybrisWebsites $HybrisWebsites -LightspeedApiKey $LightspeedApiKey -LightspeedApiSecret $LightspeedApiSecret -CommercehqApiKey $CommercehqApiKey -CommercehqApiPassword $CommercehqApiPassword -WcConsumerKey $WcConsumerKey -WcConsumerSecret $WcConsumerSecret -MagentoConsumerKey $MagentoConsumerKey -MagentoConsumerSecret $MagentoConsumerSecret -MagentoAccessToken $MagentoAccessToken -MagentoTokenSecret $MagentoTokenSecret -PrestashopWebserviceKey $PrestashopWebserviceKey -WixAppId $WixAppId -WixAppSecretKey $WixAppSecretKey -WixInstanceId $WixInstanceId -WixRefreshToken $WixRefreshToken -MercadoLibreAppId $MercadoLibreAppId -MercadoLibreAppSecretKey $MercadoLibreAppSecretKey -MercadoLibreRefreshToken $MercadoLibreRefreshToken -ZidClientId $ZidClientId -ZidClientSecret $ZidClientSecret -ZidAccessToken $ZidAccessToken -ZidAuthorization $ZidAuthorization -ZidRefreshToken $ZidRefreshToken -FlipkartClientId $FlipkartClientId -FlipkartClientSecret $FlipkartClientSecret -AllegroClientId $AllegroClientId -AllegroClientSecret $AllegroClientSecret -AllegroAccessToken $AllegroAccessToken -AllegroRefreshToken $AllegroRefreshToken -AllegroEnvironment $AllegroEnvironment -ZohoClientId $ZohoClientId -ZohoClientSecret $ZohoClientSecret -ZohoRefreshToken $ZohoRefreshToken -ZohoRegion $ZohoRegion -TiendanubeUserId $TiendanubeUserId -TiendanubeAccessToken $TiendanubeAccessToken -TiendanubeClientSecret $TiendanubeClientSecret -OttoClientId $OttoClientId -OttoClientSecret $OttoClientSecret -OttoAppId $OttoAppId -OttoRefreshToken $OttoRefreshToken -OttoEnvironment $OttoEnvironment -OttoAccessToken $OttoAccessToken -TiktokshopAppKey $TiktokshopAppKey -TiktokshopAppSecret $TiktokshopAppSecret -TiktokshopRefreshToken $TiktokshopRefreshToken -TiktokshopAccessToken $TiktokshopAccessToken -SallaClientId $SallaClientId -SallaClientSecret $SallaClientSecret -SallaRefreshToken $SallaRefreshToken -SallaAccessToken $SallaAccessToken -TemuAppKey $TemuAppKey -TemuAppSecret $TemuAppSecret -TemuAccessToken $TemuAccessToken -TemuRegion $TemuRegion
} catch {
    Write-Host ("Exception occurred when calling Invoke-AccountConfigUpdate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ReplaceParameters** | **Boolean**| Identifies if there is a necessity to replace parameters | [optional] 
 **NewStoreUrl** | **String**| The web address of the store you want to update to connect to API2Cart | [optional] 
 **NewStoreKey** | **String**| Update store key | [optional] 
 **BridgeUrl** | **String**| This parameter allows to set up store with custom bridge url (also you must use store_root parameter if a bridge folder is not in the root folder of the store) | [optional] 
 **StoreRoot** | **String**| Absolute path to the store root directory (used with &quot;&quot;bridge_url&quot;&quot; parameter) | [optional] 
 **DbTablesPrefix** | **String**| DB tables prefix | [optional] 
 **UserAgent** | **String**| This parameter allows you to set your custom user agent, which will be used in requests to the store. Please use it cautiously, as the store&#39;s firewall may block specific values. | [optional] 
 **Var3dcartPrivateKey** | **String**| 3DCart Private Key | [optional] 
 **Var3dcartAccessToken** | **String**| 3DCart Token | [optional] 
 **Var3dcartapiApiKey** | **String**| 3DCart API Key | [optional] 
 **AmazonSpClientId** | **String**| Amazon SP API app client id | [optional] 
 **AmazonSpClientSecret** | **String**| Amazon SP API app client secret | [optional] 
 **AmazonSpRefreshToken** | **String**| Amazon SP API OAuth refresh token | [optional] 
 **AmazonSpAwsRegion** | **String**| Amazon AWS Region | [optional] 
 **AmazonSpApiEnvironment** | **String**| Amazon SP API environment | [optional] [default to &quot;production&quot;]
 **AmazonSellerId** | **String**| Amazon Seller ID (Merchant token) | [optional] 
 **AspdotnetstorefrontApiUser** | **String**| It&#39;s a AspDotNetStorefront account for which API is available | [optional] 
 **AspdotnetstorefrontApiPass** | **String**| AspDotNetStorefront API Password | [optional] 
 **BigcommerceapiAdminAccount** | **String**| It&#39;s a BigCommerce account for which API is enabled | [optional] 
 **BigcommerceapiApiPath** | **String**| BigCommerce API URL | [optional] 
 **BigcommerceapiApiKey** | **String**| Bigcommerce API Key | [optional] 
 **BigcommerceapiClientId** | **String**| Client ID of the requesting app | [optional] 
 **BigcommerceapiAccessToken** | **String**| Access token authorizing the app to access resources on behalf of a user | [optional] 
 **BigcommerceapiContext** | **String**| API Path section unique to the store | [optional] 
 **BolApiKey** | **String**| Bol API Key | [optional] 
 **BolApiSecret** | **String**| Bol API Secret | [optional] 
 **BolRetailerId** | **Int32**| Bol Retailer ID | [optional] 
 **DemandwareClientId** | **String**| Demandware client id | [optional] 
 **DemandwareApiPassword** | **String**| Demandware api password | [optional] 
 **DemandwareUserName** | **String**| Demandware user name | [optional] 
 **DemandwareUserPassword** | **String**| Demandware user password | [optional] 
 **EbayClientId** | **String**| Application ID (AppID). | [optional] 
 **EbayClientSecret** | **String**| Shared Secret from eBay application | [optional] 
 **EbayRuname** | **String**| The RuName value that eBay assigns to your application. | [optional] 
 **EbayAccessToken** | **String**| Used to authenticate API requests. | [optional] 
 **EbayRefreshToken** | **String**| Used to renew the access token. | [optional] 
 **EbayEnvironment** | **String**| eBay environment | [optional] 
 **EbaySiteId** | **Int32**| eBay global ID | [optional] [default to 0]
 **EcwidAcessToken** | **String**| Access token authorizing the app to access resources on behalf of a user | [optional] 
 **EcwidStoreId** | **String**| Store Id | [optional] 
 **LazadaAppId** | **String**| Lazada App ID | [optional] 
 **LazadaAppSecret** | **String**| Lazada App Secret | [optional] 
 **LazadaRefreshToken** | **String**| Lazada Refresh Token | [optional] 
 **LazadaRegion** | **String**| Lazada API endpoint Region | [optional] 
 **EtsyKeystring** | **String**| Etsy keystring | [optional] 
 **EtsySharedSecret** | **String**| Etsy shared secret | [optional] 
 **EtsyAccessToken** | **String**| Access token authorizing the app to access resources on behalf of a user | [optional] 
 **EtsyTokenSecret** | **String**| Secret token authorizing the app to access resources on behalf of a user | [optional] 
 **EtsyClientId** | **String**| Etsy Client Id | [optional] 
 **EtsyRefreshToken** | **String**| Etsy Refresh token | [optional] 
 **FacebookAppId** | **String**| Facebook App ID | [optional] 
 **FacebookAppSecret** | **String**| Facebook App Secret | [optional] 
 **FacebookAccessToken** | **String**| Facebook Access Token | [optional] 
 **FacebookBusinessId** | **String**| Facebook Business ID | [optional] 
 **NetoApiKey** | **String**| Neto API Key | [optional] 
 **NetoApiUsername** | **String**| Neto User Name | [optional] 
 **ShoplineAccessToken** | **String**| Shopline APP Key | [optional] 
 **ShoplineAppKey** | **String**| Shopline APP Key | [optional] 
 **ShoplineAppSecret** | **String**| Shopline App Secret | [optional] 
 **ShoplineSharedSecret** | **String**| Shopline Shared Secret | [optional] 
 **ShopifyAccessToken** | **String**| Access token authorizing the app to access resources on behalf of a user | [optional] 
 **ShopifyApiKey** | **String**| Shopify API Key | [optional] 
 **ShopifyApiPassword** | **String**| Shopify API Password | [optional] 
 **ShopifySharedSecret** | **String**| Shared secret | [optional] 
 **ShopeePartnerId** | **String**| Shopee Partner ID | [optional] 
 **ShopeePartnerKey** | **String**| Shopee Partner Key | [optional] 
 **ShopeeShopId** | **String**| Shopee SHOP ID | [optional] 
 **ShopeeRefreshToken** | **String**| Shopee Refresh Token | [optional] 
 **ShopeeRegion** | **String**| Shopee API endpoint Region. Use for Chinese Mainland or Brazil. | [optional] 
 **ShopeeEnvironment** | **String**| Shopee Environment | [optional] 
 **ShoplazzaAccessToken** | **String**| Access token authorizing the app to access resources on behalf of a user | [optional] 
 **ShoplazzaSharedSecret** | **String**| Shared secret | [optional] 
 **MivaAccessToken** | **String**| Miva access token | [optional] 
 **MivaSignature** | **String**| Miva signature | [optional] 
 **ShopwareAccessKey** | **String**| Shopware access key | [optional] 
 **ShopwareApiKey** | **String**| Shopware api key | [optional] 
 **ShopwareApiSecret** | **String**| Shopware client secret access key | [optional] 
 **BigcartelUserName** | **String**| Subdomain of store | [optional] 
 **BigcartelPassword** | **String**| BigCartel account password | [optional] 
 **VolusionLogin** | **String**| It&#39;s a Volusion account for which API is enabled | [optional] 
 **VolusionPassword** | **String**| Volusion API Password | [optional] 
 **WalmartClientId** | **String**| Walmart client ID. For the region &#39;ca&#39; use Consumer ID | [optional] 
 **WalmartClientSecret** | **String**| Walmart client secret. For the region &#39;ca&#39; use Private Key | [optional] 
 **WalmartEnvironment** | **String**| Walmart environment | [optional] [default to &quot;production&quot;]
 **WalmartChannelType** | **String**| Walmart WM_CONSUMER.CHANNEL.TYPE header | [optional] 
 **WalmartRegion** | **String**| Walmart region | [optional] [default to &quot;us&quot;]
 **SquareClientId** | **String**| Square (Weebly) Client ID | [optional] 
 **SquareClientSecret** | **String**| Square (Weebly) Client Secret | [optional] 
 **SquareRefreshToken** | **String**| Square (Weebly) Refresh Token | [optional] 
 **SquarespaceApiKey** | **String**| Squarespace API Key | [optional] 
 **SquarespaceClientId** | **String**| Squarespace Connector Client ID | [optional] 
 **SquarespaceClientSecret** | **String**| Squarespace Connector Client Secret | [optional] 
 **SquarespaceAccessToken** | **String**| Squarespace access token | [optional] 
 **SquarespaceRefreshToken** | **String**| Squarespace refresh token | [optional] 
 **HybrisClientId** | **String**| Omni Commerce Connector Client ID | [optional] 
 **HybrisClientSecret** | **String**| Omni Commerce Connector Client Secret | [optional] 
 **HybrisUsername** | **String**| User Name | [optional] 
 **HybrisPassword** | **String**| User password | [optional] 
 **HybrisWebsites** | [**String[]**](String.md)| Websites to stores mapping data | [optional] 
 **LightspeedApiKey** | **String**| LightSpeed api key | [optional] 
 **LightspeedApiSecret** | **String**| LightSpeed api secret | [optional] 
 **CommercehqApiKey** | **String**| CommerceHQ api key | [optional] 
 **CommercehqApiPassword** | **String**| CommerceHQ api password | [optional] 
 **WcConsumerKey** | **String**| Woocommerce consumer key | [optional] 
 **WcConsumerSecret** | **String**| Woocommerce consumer secret | [optional] 
 **MagentoConsumerKey** | **String**| Magento Consumer Key | [optional] 
 **MagentoConsumerSecret** | **String**| Magento Consumer Secret | [optional] 
 **MagentoAccessToken** | **String**| Magento Access Token | [optional] 
 **MagentoTokenSecret** | **String**| Magento Token Secret | [optional] 
 **PrestashopWebserviceKey** | **String**| Prestashop webservice key | [optional] 
 **WixAppId** | **String**| Wix App ID | [optional] 
 **WixAppSecretKey** | **String**| Wix App Secret Key | [optional] 
 **WixInstanceId** | **String**| Wix Instance ID | [optional] 
 **WixRefreshToken** | **String**| Wix refresh token | [optional] 
 **MercadoLibreAppId** | **String**| Mercado Libre App ID | [optional] 
 **MercadoLibreAppSecretKey** | **String**| Mercado Libre App Secret Key | [optional] 
 **MercadoLibreRefreshToken** | **String**| Mercado Libre Refresh Token | [optional] 
 **ZidClientId** | **Int32**| Zid Client ID | [optional] 
 **ZidClientSecret** | **String**| Zid Client Secret | [optional] 
 **ZidAccessToken** | **String**| Zid Access Token | [optional] 
 **ZidAuthorization** | **String**| Zid Authorization | [optional] 
 **ZidRefreshToken** | **String**| Zid refresh token | [optional] 
 **FlipkartClientId** | **String**| Flipkart Client ID | [optional] 
 **FlipkartClientSecret** | **String**| Flipkart Client Secret | [optional] 
 **AllegroClientId** | **String**| Allegro Client ID | [optional] 
 **AllegroClientSecret** | **String**| Allegro Client Secret | [optional] 
 **AllegroAccessToken** | **String**| Allegro Access Token | [optional] 
 **AllegroRefreshToken** | **String**| Allegro Refresh Token | [optional] 
 **AllegroEnvironment** | **String**| Allegro Environment | [optional] [default to &quot;production&quot;]
 **ZohoClientId** | **String**| Zoho Client ID | [optional] 
 **ZohoClientSecret** | **String**| Zoho Client Secret | [optional] 
 **ZohoRefreshToken** | **String**| Zoho Refresh Token | [optional] 
 **ZohoRegion** | **String**| Zoho API endpoint Region | [optional] 
 **TiendanubeUserId** | **Int32**| Tiendanube User ID | [optional] 
 **TiendanubeAccessToken** | **String**| Tiendanube Access Token | [optional] 
 **TiendanubeClientSecret** | **String**| Tiendanube Client Secret | [optional] 
 **OttoClientId** | **String**| Otto Client ID | [optional] 
 **OttoClientSecret** | **String**| Otto Client Secret | [optional] 
 **OttoAppId** | **String**| Otto App ID | [optional] 
 **OttoRefreshToken** | **String**| Otto Refresh Token | [optional] 
 **OttoEnvironment** | **String**| Otto Environment | [optional] 
 **OttoAccessToken** | **String**| Otto Access Token | [optional] 
 **TiktokshopAppKey** | **String**| TikTok Shop App Key | [optional] 
 **TiktokshopAppSecret** | **String**| TikTok Shop App Secret | [optional] 
 **TiktokshopRefreshToken** | **String**| TikTok Shop Refresh Token | [optional] 
 **TiktokshopAccessToken** | **String**| TikTok Shop Access Token | [optional] 
 **SallaClientId** | **String**| Salla Client ID | [optional] 
 **SallaClientSecret** | **String**| Salla Client Secret | [optional] 
 **SallaRefreshToken** | **String**| Salla Refresh Token | [optional] 
 **SallaAccessToken** | **String**| Salla Access Token | [optional] 
 **TemuAppKey** | **String**| Temu App Key | [optional] 
 **TemuAppSecret** | **String**| Temu App Secret | [optional] 
 **TemuAccessToken** | **String**| Temu Access Token | [optional] 
 **TemuRegion** | **String**| Temu API endpoint Region. | [optional] 

### Return type

[**AccountConfigUpdate200Response**](AccountConfigUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AccountFailedWebhooks"></a>
# **Invoke-AccountFailedWebhooks**
> AccountFailedWebhooks200Response Invoke-AccountFailedWebhooks<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Ids] <String><br>

account.failed_webhooks

If the callback of your service for some reason could not accept webhooks from API2Cart, then with the help of this method you can get a list of missed webhooks to perform synchronization again using entity_id. Please note that we keep such records for 24 hours.

### Example
```powershell
# general setting of the PowerShell module, e.g. base URL, authentication, etc
$Configuration = Get-Configuration
# Configure API key authorization: ApiKeyAuth
$Configuration.ApiKey.x-api-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-api-key = "Bearer"

$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$Ids = "3,14,25" # String | List of сomma-separated webhook ids (optional)

# account.failed_webhooks
try {
    $Result = Invoke-AccountFailedWebhooks -Start $Start -Count $Count -Ids $Ids
} catch {
    Write-Host ("Exception occurred when calling Invoke-AccountFailedWebhooks: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **Ids** | **String**| List of сomma-separated webhook ids | [optional] 

### Return type

[**AccountFailedWebhooks200Response**](AccountFailedWebhooks200Response.md) (PSCustomObject)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AccountSupportedPlatforms"></a>
# **Invoke-AccountSupportedPlatforms**
> AccountSupportedPlatforms200Response Invoke-AccountSupportedPlatforms<br>

account.supported_platforms

Use this method to retrieve a list of supported platforms and the sets of parameters required for connecting to each of them. Note: some platforms may have multiple connection methods so that the response will contain multiple sets of parameters.

### Example
```powershell
# general setting of the PowerShell module, e.g. base URL, authentication, etc
$Configuration = Get-Configuration
# Configure API key authorization: ApiKeyAuth
$Configuration.ApiKey.x-api-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-api-key = "Bearer"


# account.supported_platforms
try {
    $Result = Invoke-AccountSupportedPlatforms
} catch {
    Write-Host ("Exception occurred when calling Invoke-AccountSupportedPlatforms: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AccountSupportedPlatforms200Response**](AccountSupportedPlatforms200Response.md) (PSCustomObject)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

