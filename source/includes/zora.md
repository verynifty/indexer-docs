# Zora Marketplace Data

## Get active Asks for owner

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/zora/asks/owner/0x35F36467CA7c6d1B4e33E5d183AEf9a01486efa7"
);
```

```json
{
   "asks":[
      {
         "block_number":"14490562",
         "timestamp":"2022-03-30T23:49:14.000Z",
         "log_index":"431",
         "transaction_hash":"0x4bcbf7c9618e4ede1e5583f46739e707bcf04d5527ecaaf6b3113719c70bc2a9",
         "address":"0xa7f636adf14512199716688b33a069dbcb6d5766",
         "token_id":"4339",
         "status":0,
         "buyer":null,
         "finder":null,
         "seller":"0x08f8d3aaa03043690b0f2f8d001f722534ffbc5e",
         "seller_funds_recipient":"0x08f8d3aaa03043690b0f2f8d001f722534ffbc5e",
         "currency":null,
         "price":"1000000000000000000",
         "fee":"200",
         "nft":{
            "address":"0xa7f636adf14512199716688b33a069dbcb6d5766",
            "token_id":4339,
            "name":"Dank Ducks #4339",
            "description":"6,969 of the dankest ducks floating in the metaverse.",
            "external_url":"https://gateway.ipfs.io/ipfs/QmXS9Sfn7rQiod4ZppqEsWEX3UJUoiTTAnqPv7VBuKt1Fq/4339.json",
            "original_image":"https://gateway.ipfs.io/ipfs/Qma8T1FABPJqjrPvzknyHwTW8Myg4teWdFE1FEowshb6Mt/4339.png",
            "image":"https://media.niftyapi.xyz/0xa7f636adf14512199716688b33a069dbcb6d5766/4339",
            "original_animation":null,
            "attributes":{
               "Body":"Base",
               "Hats":"Gray_Cat_Hat",
               "Faces":"Happy",
               "Clothes":"White_Tuxedo",
               "Backgrounds":"Uncommon"
            },
            "metadata_type":5,
            "image_type":4,
            "owner":"0x08f8d3aaa03043690b0f2f8d001f722534ffbc5e",
            "created_at":"2022-03-25T14:59:43.210581",
            "updated_at":"2022-05-29T01:13:09.837633",
            "latest_block_number":14863589,
            "latest_log_index":509
         }
      }
   ]
}
```

This endpoint returns active asks created by user address

### HTTP Request

`GET https://api.niftyapi.xyz/zora/asks/owner/:address`

### URL Parameters
| Parameter | Description                          |
| --------- | ------------------------------------ |
| Address   | The user address to retrieve active asks from |


## Get active Ask for NFT

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/zora/ask/0xa7d8d9ef8D8Ce8992Df33D8b8CF4Aebabd5bD270/205000237"
);
```

```json
{
   "asks":[
      {
         "block_number":"14490562",
         "timestamp":"2022-03-30T23:49:14.000Z",
         "log_index":"431",
         "transaction_hash":"0x4bcbf7c9618e4ede1e5583f46739e707bcf04d5527ecaaf6b3113719c70bc2a9",
         "address":"0xa7f636adf14512199716688b33a069dbcb6d5766",
         "token_id":"4339",
         "status":0,
         "buyer":null,
         "finder":null,
         "seller":"0x08f8d3aaa03043690b0f2f8d001f722534ffbc5e",
         "seller_funds_recipient":"0x08f8d3aaa03043690b0f2f8d001f722534ffbc5e",
         "currency":null,
         "price":"1000000000000000000",
         "fee":"200",
         "nft":{
            "address":"0xa7f636adf14512199716688b33a069dbcb6d5766",
            "token_id":4339,
            "name":"Dank Ducks #4339",
            "description":"6,969 of the dankest ducks floating in the metaverse.",
            "external_url":"https://gateway.ipfs.io/ipfs/QmXS9Sfn7rQiod4ZppqEsWEX3UJUoiTTAnqPv7VBuKt1Fq/4339.json",
            "original_image":"https://gateway.ipfs.io/ipfs/Qma8T1FABPJqjrPvzknyHwTW8Myg4teWdFE1FEowshb6Mt/4339.png",
            "image":"https://media.niftyapi.xyz/0xa7f636adf14512199716688b33a069dbcb6d5766/4339",
            "original_animation":null,
            "attributes":{
               "Body":"Base",
               "Hats":"Gray_Cat_Hat",
               "Faces":"Happy",
               "Clothes":"White_Tuxedo",
               "Backgrounds":"Uncommon"
            },
            "metadata_type":5,
            "image_type":4,
            "owner":"0x08f8d3aaa03043690b0f2f8d001f722534ffbc5e",
            "created_at":"2022-03-25T14:59:43.210581",
            "updated_at":"2022-05-29T01:13:09.837633",
            "latest_block_number":14863589,
            "latest_log_index":509
         }
      }
   ]
}
```

This endpoint returns active asks created by user address

### HTTP Request

`GET https://api.niftyapi.xyz/zora/ask/collection/:token_id`

### URL Parameters
| Parameter | Description                          |
| --------- | ------------------------------------ |
| collection   | Collection address of NFT |
| token_id   | The token id for NFT |

## Ask for Collection

This endpoint returns internal server error
https://api.niftyapi.xyz/zora/ask/collection/:collection

## Get active Offers created by owner

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/zora/offers/maker/0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4"
);
```

```json
{
   "offers":[
      {
         "block_number":"14450575",
         "timestamp":"2022-03-24T18:24:00.000Z",
         "log_index":"478",
         "transaction_hash":"0x7802a9e6c815b04ec5f23ee0c10ff89526e75799b069ab98b01060981840db2a",
         "offer_id":"1",
         "address":"0x0144b7e66993c6bfab85581e8601f96bfe50c9df",
         "token_id":"3660",
         "status":0,
         "buyer":null,
         "finder":null,
         "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "currency":null,
         "price":"1000000000000000",
         "fee":"0",
         "nft":{
            "address":"0x0144b7e66993c6bfab85581e8601f96bfe50c9df",
            "token_id":3660,
            "name":"Pride Punk #3660",
            "description":"The first Punk Derivative",
            "external_url":"https://gateway.ipfs.io/ipfs/bafybeihuwyzyxmghhgbk5jvu4rjzwworbnvkfh6ba4pm3xrxb6iovnguhq/3660",
            "original_image":"https://gateway.ipfs.io/ipfs/bafkreieybuanpguxvashei3e2qk5throlefsboazvr6joc2cblwmqemuwy",
            "image":"https://media.niftyapi.xyz/0x0144b7e66993c6bfab85581e8601f96bfe50c9df/3660",
            "original_animation":null,
            "attributes":{
               "type":"Male",
               "accessory":"2 attributes"
            },
            "metadata_type":5,
            "image_type":4,
            "owner":"0xca72b32a2ec25eae54db599714cac0175bbccba5",
            "created_at":"2022-03-24T00:49:50.24816",
            "updated_at":"2022-04-10T13:06:28.184697",
            "latest_block_number":14558105,
            "latest_log_index":278
         }
      }
   ]
}
```

This endpoint returns active offers created by user address

### HTTP Request

`GET https://api.niftyapi.xyz/zora/offers/owner/:address`

### URL Parameters
| Parameter | Description                                         |
| --------- | --------------------------------------------------- |
| Address   | The user address to retrieve all active offers from |

## Get all active offers for NFT

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/zora/offers/nft/0x0144b7e66993c6bfab85581e8601f96bfe50c9df/3660"
);
```

```json
{
   "offers":[
      {
         "block_number":"14450575",
         "timestamp":"2022-03-24T18:24:00.000Z",
         "log_index":"478",
         "transaction_hash":"0x7802a9e6c815b04ec5f23ee0c10ff89526e75799b069ab98b01060981840db2a",
         "offer_id":"1",
         "address":"0x0144b7e66993c6bfab85581e8601f96bfe50c9df",
         "token_id":"3660",
         "status":0,
         "buyer":null,
         "finder":null,
         "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "currency":null,
         "price":"1000000000000000",
         "fee":"0",
         "nft":{
            "address":"0x0144b7e66993c6bfab85581e8601f96bfe50c9df",
            "token_id":3660,
            "name":"Pride Punk #3660",
            "description":"The first Punk Derivative",
            "external_url":"https://gateway.ipfs.io/ipfs/bafybeihuwyzyxmghhgbk5jvu4rjzwworbnvkfh6ba4pm3xrxb6iovnguhq/3660",
            "original_image":"https://gateway.ipfs.io/ipfs/bafkreieybuanpguxvashei3e2qk5throlefsboazvr6joc2cblwmqemuwy",
            "image":"https://media.niftyapi.xyz/0x0144b7e66993c6bfab85581e8601f96bfe50c9df/3660",
            "original_animation":null,
            "attributes":{
               "type":"Male",
               "accessory":"2 attributes"
            },
            "metadata_type":5,
            "image_type":4,
            "owner":"0xca72b32a2ec25eae54db599714cac0175bbccba5",
            "created_at":"2022-03-24T00:49:50.24816",
            "updated_at":"2022-04-10T13:06:28.184697",
            "latest_block_number":14558105,
            "latest_log_index":278
         }
      }
   ]
}
```

This endpoint returns all active offers for NFT

### HTTP Request

`GET https://api.niftyapi.xyz/zora/offers/nft/:collection/:token_id`

### URL Parameters
| Parameter | Description                                         |
| --------- | --------------------------------------------------- |
| collection | Collection address of NFT |
| token_id | Token id of NFT |

## Get all active offers for collection

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/zora/offers/collection/0x0144b7e66993c6bfab85581e8601f96bfe50c9df"
);
```

```json
{
   "offers":[
      {
         "block_number":"14450575",
         "timestamp":"2022-03-24T18:24:00.000Z",
         "log_index":"478",
         "transaction_hash":"0x7802a9e6c815b04ec5f23ee0c10ff89526e75799b069ab98b01060981840db2a",
         "offer_id":"1",
         "address":"0x0144b7e66993c6bfab85581e8601f96bfe50c9df",
         "token_id":"3660",
         "status":0,
         "buyer":null,
         "finder":null,
         "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "currency":null,
         "price":"1000000000000000",
         "fee":"0",
         "nft":{
            "address":"0x0144b7e66993c6bfab85581e8601f96bfe50c9df",
            "token_id":3660,
            "name":"Pride Punk #3660",
            "description":"The first Punk Derivative",
            "external_url":"https://gateway.ipfs.io/ipfs/bafybeihuwyzyxmghhgbk5jvu4rjzwworbnvkfh6ba4pm3xrxb6iovnguhq/3660",
            "original_image":"https://gateway.ipfs.io/ipfs/bafkreieybuanpguxvashei3e2qk5throlefsboazvr6joc2cblwmqemuwy",
            "image":"https://media.niftyapi.xyz/0x0144b7e66993c6bfab85581e8601f96bfe50c9df/3660",
            "original_animation":null,
            "attributes":{
               "type":"Male",
               "accessory":"2 attributes"
            },
            "metadata_type":5,
            "image_type":4,
            "owner":"0xca72b32a2ec25eae54db599714cac0175bbccba5",
            "created_at":"2022-03-24T00:49:50.24816",
            "updated_at":"2022-04-10T13:06:28.184697",
            "latest_block_number":14558105,
            "latest_log_index":278
         }
      }
   ]
}
```

This endpoint returns all active offers for collection

### HTTP Request

`GET https://api.niftyapi.xyz/zora/offers/nft/:collection`

### URL Parameters
| Parameter | Description                                         |
| --------- | --------------------------------------------------- |
| collection | Collection address to get all active offers for |

## Get activity for user

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/zora/activity/address/0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4"
);
```

```json
[
   {
      "type":"ask",
      "status":"AskCreatedOrUpdated",
      "block_number":"14463626",
      "log_index":"578",
      "timestamp":"2022-03-26T19:08:20.000Z",
      "transaction_hash":"0xb2f3063291149b5cabde5321680170a099d0e2b82c60206dae79f472e451a74c",
      "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
      "token_id":"0",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"1000000000000000000000",
      "nft":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "token_id":0,
         "name":"Dreams of EVM #0",
         "description":null,
         "external_url":"data:application/json;utf8,{\"name\":\"Dreams of EVM #0\",\"image\": \"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>\", \"attributes\":[{\"trait_type\": \"Color\",\"value\":\"Lava\"},{\"trait_type\": \"Level\",\"value\":\"1\"},{\"trait_type\": \"Rotate\",\"value\":\"45\"}]}",
         "original_image":"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>",
         "image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/0",
         "original_animation":null,
         "attributes":{
            "Color":"Lava",
            "Level":"1",
            "Rotate":"45"
         },
         "metadata_type":2,
         "image_type":3,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:21:08.175443",
         "updated_at":"2022-04-01T09:29:07.828044",
         "latest_block_number":13274859,
         "latest_log_index":88
      },
      "collection":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "name":"Dreams of EVM",
         "symbol":"EVM",
         "default_image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/12",
         "slug":"dreams-of-evm",
         "decimals":1,
         "first_block_seen":14074459,
         "type":721,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:20:56.508232",
         "nft_data_base_url":null,
         "nft_image_base_url":null,
         "transfers_total":319,
         "metadata":null,
         "first_transfer":"2021-09-22T09:46:26"
      }
   },
   {
      "type":"ask",
      "status":"AskCanceled",
      "block_number":"14463626",
      "log_index":"577",
      "timestamp":"2022-03-26T19:08:20.000Z",
      "transaction_hash":"0xb2f3063291149b5cabde5321680170a099d0e2b82c60206dae79f472e451a74c",
      "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
      "token_id":"0",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"10000000000000000000000",
      "nft":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "token_id":0,
         "name":"Dreams of EVM #0",
         "description":null,
         "external_url":"data:application/json;utf8,{\"name\":\"Dreams of EVM #0\",\"image\": \"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>\", \"attributes\":[{\"trait_type\": \"Color\",\"value\":\"Lava\"},{\"trait_type\": \"Level\",\"value\":\"1\"},{\"trait_type\": \"Rotate\",\"value\":\"45\"}]}",
         "original_image":"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>",
         "image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/0",
         "original_animation":null,
         "attributes":{
            "Color":"Lava",
            "Level":"1",
            "Rotate":"45"
         },
         "metadata_type":2,
         "image_type":3,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:21:08.175443",
         "updated_at":"2022-04-01T09:29:07.828044",
         "latest_block_number":13274859,
         "latest_log_index":88
      },
      "collection":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "name":"Dreams of EVM",
         "symbol":"EVM",
         "default_image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/12",
         "slug":"dreams-of-evm",
         "decimals":1,
         "first_block_seen":14074459,
         "type":721,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:20:56.508232",
         "nft_data_base_url":null,
         "nft_image_base_url":null,
         "transfers_total":319,
         "metadata":null,
         "first_transfer":"2021-09-22T09:46:26"
      }
   },
   {
      "type":"ask",
      "status":"AskCreatedOrUpdated",
      "block_number":"14463623",
      "log_index":"442",
      "timestamp":"2022-03-26T19:07:32.000Z",
      "transaction_hash":"0x618bc405947f9b77235fb96a3c34bccd8f3d53785497fe8810228ef4678e0b66",
      "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
      "token_id":"0",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"10000000000000000000000",
      "nft":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "token_id":0,
         "name":"Dreams of EVM #0",
         "description":null,
         "external_url":"data:application/json;utf8,{\"name\":\"Dreams of EVM #0\",\"image\": \"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>\", \"attributes\":[{\"trait_type\": \"Color\",\"value\":\"Lava\"},{\"trait_type\": \"Level\",\"value\":\"1\"},{\"trait_type\": \"Rotate\",\"value\":\"45\"}]}",
         "original_image":"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>",
         "image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/0",
         "original_animation":null,
         "attributes":{
            "Color":"Lava",
            "Level":"1",
            "Rotate":"45"
         },
         "metadata_type":2,
         "image_type":3,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:21:08.175443",
         "updated_at":"2022-04-01T09:29:07.828044",
         "latest_block_number":13274859,
         "latest_log_index":88
      },
      "collection":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "name":"Dreams of EVM",
         "symbol":"EVM",
         "default_image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/12",
         "slug":"dreams-of-evm",
         "decimals":1,
         "first_block_seen":14074459,
         "type":721,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:20:56.508232",
         "nft_data_base_url":null,
         "nft_image_base_url":null,
         "transfers_total":319,
         "metadata":null,
         "first_transfer":"2021-09-22T09:46:26"
      }
   },
   {
      "type":"ask",
      "status":"AskCanceled",
      "block_number":"14463623",
      "log_index":"441",
      "timestamp":"2022-03-26T19:07:32.000Z",
      "transaction_hash":"0x618bc405947f9b77235fb96a3c34bccd8f3d53785497fe8810228ef4678e0b66",
      "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
      "token_id":"0",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"1000000000000000000000",
      "nft":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "token_id":0,
         "name":"Dreams of EVM #0",
         "description":null,
         "external_url":"data:application/json;utf8,{\"name\":\"Dreams of EVM #0\",\"image\": \"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>\", \"attributes\":[{\"trait_type\": \"Color\",\"value\":\"Lava\"},{\"trait_type\": \"Level\",\"value\":\"1\"},{\"trait_type\": \"Rotate\",\"value\":\"45\"}]}",
         "original_image":"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>",
         "image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/0",
         "original_animation":null,
         "attributes":{
            "Color":"Lava",
            "Level":"1",
            "Rotate":"45"
         },
         "metadata_type":2,
         "image_type":3,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:21:08.175443",
         "updated_at":"2022-04-01T09:29:07.828044",
         "latest_block_number":13274859,
         "latest_log_index":88
      },
      "collection":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "name":"Dreams of EVM",
         "symbol":"EVM",
         "default_image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/12",
         "slug":"dreams-of-evm",
         "decimals":1,
         "first_block_seen":14074459,
         "type":721,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:20:56.508232",
         "nft_data_base_url":null,
         "nft_image_base_url":null,
         "transfers_total":319,
         "metadata":null,
         "first_transfer":"2021-09-22T09:46:26"
      }
   },
   {
      "type":"ask",
      "status":"AskCreatedOrUpdated",
      "block_number":"14463621",
      "log_index":"146",
      "timestamp":"2022-03-26T19:07:09.000Z",
      "transaction_hash":"0x84575788fe20fa81cff634c30d924982829397fd66905bd5676b4a11ffa93dce",
      "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
      "token_id":"0",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"1000000000000000000000",
      "nft":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "token_id":0,
         "name":"Dreams of EVM #0",
         "description":null,
         "external_url":"data:application/json;utf8,{\"name\":\"Dreams of EVM #0\",\"image\": \"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>\", \"attributes\":[{\"trait_type\": \"Color\",\"value\":\"Lava\"},{\"trait_type\": \"Level\",\"value\":\"1\"},{\"trait_type\": \"Rotate\",\"value\":\"45\"}]}",
         "original_image":"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>",
         "image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/0",
         "original_animation":null,
         "attributes":{
            "Color":"Lava",
            "Level":"1",
            "Rotate":"45"
         },
         "metadata_type":2,
         "image_type":3,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:21:08.175443",
         "updated_at":"2022-04-01T09:29:07.828044",
         "latest_block_number":13274859,
         "latest_log_index":88
      },
      "collection":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "name":"Dreams of EVM",
         "symbol":"EVM",
         "default_image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/12",
         "slug":"dreams-of-evm",
         "decimals":1,
         "first_block_seen":14074459,
         "type":721,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:20:56.508232",
         "nft_data_base_url":null,
         "nft_image_base_url":null,
         "transfers_total":319,
         "metadata":null,
         "first_transfer":"2021-09-22T09:46:26"
      }
   },
   {
      "type":"ask",
      "status":"AskCanceled",
      "block_number":"14463621",
      "log_index":"145",
      "timestamp":"2022-03-26T19:07:09.000Z",
      "transaction_hash":"0x84575788fe20fa81cff634c30d924982829397fd66905bd5676b4a11ffa93dce",
      "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
      "token_id":"0",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"1000000000000000000000",
      "nft":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "token_id":0,
         "name":"Dreams of EVM #0",
         "description":null,
         "external_url":"data:application/json;utf8,{\"name\":\"Dreams of EVM #0\",\"image\": \"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>\", \"attributes\":[{\"trait_type\": \"Color\",\"value\":\"Lava\"},{\"trait_type\": \"Level\",\"value\":\"1\"},{\"trait_type\": \"Rotate\",\"value\":\"45\"}]}",
         "original_image":"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>",
         "image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/0",
         "original_animation":null,
         "attributes":{
            "Color":"Lava",
            "Level":"1",
            "Rotate":"45"
         },
         "metadata_type":2,
         "image_type":3,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:21:08.175443",
         "updated_at":"2022-04-01T09:29:07.828044",
         "latest_block_number":13274859,
         "latest_log_index":88
      },
      "collection":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "name":"Dreams of EVM",
         "symbol":"EVM",
         "default_image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/12",
         "slug":"dreams-of-evm",
         "decimals":1,
         "first_block_seen":14074459,
         "type":721,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:20:56.508232",
         "nft_data_base_url":null,
         "nft_image_base_url":null,
         "transfers_total":319,
         "metadata":null,
         "first_transfer":"2021-09-22T09:46:26"
      }
   },
   {
      "type":"ask",
      "status":"AskCreatedOrUpdated",
      "block_number":"14463583",
      "log_index":"71",
      "timestamp":"2022-03-26T19:01:14.000Z",
      "transaction_hash":"0x957c44ebd22ab1e877b8c85abb86fa0c9b1345016da068190bd71672c91e824c",
      "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
      "token_id":"0",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"1000000000000000000000",
      "nft":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "token_id":0,
         "name":"Dreams of EVM #0",
         "description":null,
         "external_url":"data:application/json;utf8,{\"name\":\"Dreams of EVM #0\",\"image\": \"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>\", \"attributes\":[{\"trait_type\": \"Color\",\"value\":\"Lava\"},{\"trait_type\": \"Level\",\"value\":\"1\"},{\"trait_type\": \"Rotate\",\"value\":\"45\"}]}",
         "original_image":"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#F8FF00'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#B33607; #FFFA27; #B33607' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#FFFA27; #B33607; #FFFA27' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(1)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='1; 0.7; 1' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(45 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#F8FF00'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#FFFA27' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#FFFA27' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#FFFA27' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#FFFA27' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#FFFA27'>EVM Dreams #0 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>",
         "image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/0",
         "original_animation":null,
         "attributes":{
            "Color":"Lava",
            "Level":"1",
            "Rotate":"45"
         },
         "metadata_type":2,
         "image_type":3,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:21:08.175443",
         "updated_at":"2022-04-01T09:29:07.828044",
         "latest_block_number":13274859,
         "latest_log_index":88
      },
      "collection":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "name":"Dreams of EVM",
         "symbol":"EVM",
         "default_image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/12",
         "slug":"dreams-of-evm",
         "decimals":1,
         "first_block_seen":14074459,
         "type":721,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:20:56.508232",
         "nft_data_base_url":null,
         "nft_image_base_url":null,
         "transfers_total":319,
         "metadata":null,
         "first_transfer":"2021-09-22T09:46:26"
      }
   },
   {
      "type":"ask",
      "status":"AskCreatedOrUpdated",
      "block_number":"14463317",
      "log_index":"357",
      "timestamp":"2022-03-26T17:57:03.000Z",
      "transaction_hash":"0xbc113edf05c27981d67553166992bc06e0285221dcc371c35a7a0519d095c0a6",
      "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
      "token_id":"1",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"100000000000000000000",
      "nft":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "token_id":1,
         "name":"Dreams of EVM #1",
         "description":null,
         "external_url":"data:application/json;utf8,{\"name\":\"Dreams of EVM #1\",\"image\": \"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#ecf0f1'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#c99d66; #333333; #c99d66' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#333333; #c99d66; #333333' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(2)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='2; 0.7; 2' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(34 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#ecf0f1'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#333333' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#333333' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#333333' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#333333' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#333333'>EVM Dreams #1 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>\", \"attributes\":[{\"trait_type\": \"Color\",\"value\":\"Hot Koala\"},{\"trait_type\": \"Level\",\"value\":\"2\"},{\"trait_type\": \"Rotate\",\"value\":\"34\"}]}",
         "original_image":"data:image/svg+xml;utf8,<svg version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' viewBox='0 0 1000 1000' width='1000' height='1000' fill='#ecf0f1'><defs><filter id='f1' x='0' y='0'><feGaussianBlur in='SourceGraphic' stdDeviation='0.2' /></filter><linearGradient id='gr' gradientTransform='rotate(90)'><stop offset='5%'><animate attributeName='stop-color' values='#c99d66; #333333; #c99d66' dur='10' repeatCount='indefinite'></animate></stop><stop offset='70%'><animate attributeName='stop-color' values='#333333; #c99d66; #333333' dur='9s' repeatCount='indefinite'></animate></stop></linearGradient><pattern id='t' patternUnits='userSpaceOnUse' width='562.6' height='325' patternTransform='scale(2)' stroke='url(#gr)'  stroke-width='8'><animateTransform attributeName='patternTransform' type='scale' dur='70s' values='2; 0.7; 2' repeatCount='indefinite'/><animate attributeName='stroke-width' values='2; 10; 2' dur='15s' repeatCount='indefinite'/><g id='g'><polygon points='281.4,0 375.2, 162.5 281.4, 325 187, 161.5'  id='b'/><g id='B'><use xlink:href='#b' transform='rotate(34 280 162.5) translate(116, 67) scale(.58)' id='b1'/><g id='d'><use xlink:href='#b' transform='translate(188.85, 108) scale(.33)' id='b2'/><g id='sd'><use xlink:href='#b1' transform='translate(189.85, 108) scale(.33)' id='b3'/><use xlink:href='#b2' transform='translate(188.85, 108) scale(.33)' id='b4'/><use xlink:href='#b3' transform='translate(188.85, 108) scale(.33)'/><use xlink:href='#b4' transform='translate(188.85, 108) scale(.33)'/></g></g><use xlink:href='#sd' transform='translate(62,0)'/><use xlink:href='#sd' transform='translate(-62,0)'/><use xlink:href='#d' transform='translate(0,-107)'/><use xlink:href='#d' transform='translate(0, 107)'/></g></g><g id='t'><use xlink:href='#g'/><use xlink:href='#g' transform='rotate(60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 0)'/><use xlink:href='#g' transform='rotate(-60 281 325)'/><use xlink:href='#g' transform='rotate(60 281 325)'/><g id='v'><use xlink:href='#g' transform='translate(-282, -162)'/><use xlink:href='#g' transform='translate(-282, 162)'/></g><use xlink:href='#v' transform='translate(564, 0)'/></g></pattern></defs><rect width='100%' height='100%' fill='#ecf0f1'/><rect width='980' x='10' y='10' height='980' fill='url(#t)'/><line x1='0' y1='10' x2='1000' y2='10' stroke='#333333' /><line x1='0' y1='990' x2='1000' y2='990' stroke='#333333' /><line x1='10' y1='0' x2='10' y2='1000' stroke='#333333' /><line x1='990' y1='0' x2='990' y2='1000' stroke='#333333' /><text x='12' y='999' class='small' font-family='monospace' font-size='10' fill='#333333'>EVM Dreams #1 | Can t be described in the same way that one might point to a cloud or an ocean wave, but it does exist as one single entity</text></svg>",
         "image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/1",
         "original_animation":null,
         "attributes":{
            "Color":"Hot Koala",
            "Level":"2",
            "Rotate":"34"
         },
         "metadata_type":2,
         "image_type":3,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:21:08.376611",
         "updated_at":"2022-04-01T09:29:08.110426",
         "latest_block_number":13684907,
         "latest_log_index":501
      },
      "collection":{
         "address":"0x10e0271ec47d55511a047516f2a7301801d55eab",
         "name":"Dreams of EVM",
         "symbol":"EVM",
         "default_image":"https://media.niftyapi.xyz/0x10e0271ec47d55511a047516f2a7301801d55eab/12",
         "slug":"dreams-of-evm",
         "decimals":1,
         "first_block_seen":14074459,
         "type":721,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T11:20:56.508232",
         "nft_data_base_url":null,
         "nft_image_base_url":null,
         "transfers_total":319,
         "metadata":null,
         "first_transfer":"2021-09-22T09:46:26"
      }
   },
   {
      "type":"ask",
      "status":"AskCreatedOrUpdated",
      "block_number":"14450607",
      "log_index":"191",
      "timestamp":"2022-03-24T18:32:16.000Z",
      "transaction_hash":"0xd61f6a497f66a40ecf2a15d68111e12b7c9e97c396eca94d6e48baf21c91ada4",
      "address":"0xc3f733ca98e0dad0386979eb96fb1722a1a05e69",
      "token_id":"6481",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"200000000000000000000",
      "nft":{
         "address":"0xc3f733ca98e0dad0386979eb96fb1722a1a05e69",
         "token_id":6481,
         "name":"MoonCat #6481: 0x00802c2a76 (accessorized)",
         "description":"An Adorable Pure Pale Blue/Sky Blue Smiling [MoonCat](https://purrse.mooncat.community/6481).",
         "external_url":"https://api.mooncat.community/traits/6481",
         "original_image":"https://api.mooncat.community/image/0x00802c2a76",
         "image":"https://media.niftyapi.xyz/0xc3f733ca98e0dad0386979eb96fb1722a1a05e69/6481",
         "original_animation":"https://api.mooncat.community/dynamic/0x00802c2a76",
         "attributes":{
            "Hue":"241",
            "Coat":"Pale Blue Pure",
            "Pose":"Standing",
            "isNamed":"No",
            "Coat Hue":"Blue",
            "Accessory":"#702: vNFT Mask 1",
            "lootprint":"Minted",
            "Expression":"Smiling",
            "Has Twins?":"Yes",
            "MoonCat Id":"0x00802c2a76",
            "Has Clones?":"No",
            "Only Child?":"No",
            "Rescue Year":"2021",
            "Coat Pattern":"Pure",
            "Has Mirrors?":"No",
            "Rescue Index":"6481",
            "Classification":"Rescue",
            "Coat Saturation":"Pale",
            "Total Accessories":"5"
         },
         "metadata_type":1,
         "image_type":1,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-24T12:20:55.410636",
         "updated_at":"2022-05-12T23:25:48.125239",
         "latest_block_number":13798484,
         "latest_log_index":119
      },
      "collection":{
         "address":"0xc3f733ca98e0dad0386979eb96fb1722a1a05e69",
         "name":"MoonCats",
         "symbol":"😺",
         "default_image":"https://media.niftyapi.xyz/0xc3f733ca98e0dad0386979eb96fb1722a1a05e69/21226",
         "slug":"acclimatedmooncats",
         "decimals":1,
         "first_block_seen":14000651,
         "type":721,
         "owner":"0xd342a4f0397b4268e6adce89b9b88c746afa85ee",
         "created_at":"2022-01-14T01:26:52.296323",
         "nft_data_base_url":"https://api.mooncat.community/traits/__TOKENID__",
         "nft_image_base_url":null,
         "transfers_total":49774,
         "metadata":{
            "website":"https://mooncat.community",
            "image_url":"https://lh3.googleusercontent.com/RwIPOH0RftzOWtyC0WBnMx2X4_4Xqeimk5iT6I1xNQKSuRTVNwBY0PcA6MkCiX2dVP5U_MDbseAq3LoaJ7BY_xyTfLpeUsGtt2-WTA=s120",
            "description":"Launched on August 10th, 2017, the MoonCatRescue Insanely Cute Operation was a success! The 25440 MoonCats rescued are acclimating to their life as [fully on-chain](https://mooncat.community/about) collectible critters.\r\n\r\nVintage, generative, and a pioneer of fair distribution, MoonCats can also be customized in the on-chain [MoonCatBoutique](https://boutique.mooncat.community)!\r\n\r\nOwners have [Personal and Commercial License](https://mooncat.community/mooncatlicense) to their MoonCat's imagery.",
            "discord_url":"https://discord.gg/mooncats",
            "medium_username":"mooncatcommunity",
            "banner_image_url":"https://lh3.googleusercontent.com/GqVjY5pCGyHzfo5zYl6ocRbdEGGwZPgXcmyKCcPMhepkZATScV6H_iKlGvnkyfgLE_QdpFLHUeYhzMCHPGMGpKwKXuVL4vbuFMPD0A=s2500",
            "twitter_username":"ponderware",
            "featured_image_url":"https://lh3.googleusercontent.com/kIfTnHDRFqRIOg1jkPoaD9oNwhOdLk2_0MOy1SqG2iqkWxiZ0FRq5ZFXjHCQKUmIoUAZxHzhAA43cd9vmr1Geuu1pSryXO5BHEihKt8=s300"
         },
         "first_transfer":"2021-04-22T03:17:13"
      }
   },
   {
      "type":"offer",
      "status":"OfferCreatedOrUpdated",
      "block_number":"14450575",
      "log_index":"478",
      "timestamp":"2022-03-24T18:24:00.000Z",
      "transaction_hash":"0x7802a9e6c815b04ec5f23ee0c10ff89526e75799b069ab98b01060981840db2a",
      "address":"0x0144b7e66993c6bfab85581e8601f96bfe50c9df",
      "token_id":"3660",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"1000000000000000",
      "nft":{
         "address":"0x0144b7e66993c6bfab85581e8601f96bfe50c9df",
         "token_id":3660,
         "name":"Pride Punk #3660",
         "description":"The first Punk Derivative",
         "external_url":"https://gateway.ipfs.io/ipfs/bafybeihuwyzyxmghhgbk5jvu4rjzwworbnvkfh6ba4pm3xrxb6iovnguhq/3660",
         "original_image":"https://gateway.ipfs.io/ipfs/bafkreieybuanpguxvashei3e2qk5throlefsboazvr6joc2cblwmqemuwy",
         "image":"https://media.niftyapi.xyz/0x0144b7e66993c6bfab85581e8601f96bfe50c9df/3660",
         "original_animation":null,
         "attributes":{
            "type":"Male",
            "accessory":"2 attributes"
         },
         "metadata_type":5,
         "image_type":4,
         "owner":"0xca72b32a2ec25eae54db599714cac0175bbccba5",
         "created_at":"2022-03-24T00:49:50.24816",
         "updated_at":"2022-04-10T13:06:28.184697",
         "latest_block_number":14558105,
         "latest_log_index":278
      },
      "collection":{
         "address":"0x0144b7e66993c6bfab85581e8601f96bfe50c9df",
         "name":"PridePunks 2018",
         "symbol":"MP",
         "default_image":"https://media.niftyapi.xyz/0x0144b7e66993c6bfab85581e8601f96bfe50c9df/0",
         "slug":"pridepunks2018",
         "decimals":1,
         "first_block_seen":14303869,
         "type":721,
         "owner":"0xe8d848debb3a3e12aa815b15900c8e020b863f31",
         "created_at":"2022-03-01T22:34:09.471895",
         "nft_data_base_url":"https://ipfs.io/ipfs/bafybeigmfmrekuq65vhsiypvmdj3zhxwa2w7jic2z7dx4vrggqj2o6cuhq/__TOKENID__",
         "nft_image_base_url":null,
         "transfers_total":27884,
         "metadata":{
            "website":"http://pridepunk.xyz",
            "image_url":"https://lh3.googleusercontent.com/DWKOSDqHY5BpP9lnXTn2Cmb5OEwzvVT01nZNwSxwzA8qXaLuagOXVaszkMcxXe6BNIGlx8CdKMzhPahwm6x21NX2p-LbsmBGBGqQ=s120",
            "description":"The FIRST CryptoPunks Derivative, in 2018!\r\n\r\n\r\nProof: (LarvaLabs Discord Announcement) https://discord.com/channels/329381334701178885/329381334701178885/460157631437340693\r\nProof: (2018 Smart Contract) https://etherscan.io/address/0x0144b7e66993c6bfab85581e8601f96bfe50c9df#code\r\n\r\nCreated as a statement on diversity in Web3, now a legitimate historical NFT.",
            "discord_url":"https://discord.gg/mnYJKxMgaU",
            "banner_image_url":"https://lh3.googleusercontent.com/weuzocbwyBu_vFwZ5BilZ7cjbk0ZPEfLCkZSE7AAO_5-q43WRgcxRQhq9gE6IvtANDXkjfI5-BInomGH8yWa_6btVCJVzGUZJaTgjQ=s2500",
            "featured_image_url":"https://lh3.googleusercontent.com/rQWHSLfzLM2HerdgsxDKBXt-NoeZbz3YOsvChohAXXooT__NmQMpgM1O2cI1EJguQUcYtV4DNpAlVxKTu3O-7S6PAJw3a6pnq0ke=s300"
         },
         "first_transfer":"2022-03-01T22:32:54"
      }
   },
   {
      "type":"ask",
      "status":"AskCreatedOrUpdated",
      "block_number":"14360255",
      "log_index":"291",
      "timestamp":"2022-03-10T16:48:33.000Z",
      "transaction_hash":"0x156919cc418c37185c9685057215fd25a061bdf9c54c46dd6d5f0aa5873bae22",
      "address":"0x4961db588dd962abb20927aa38fa33e5225b3be2",
      "token_id":"2928",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"100000000000000000000",
      "nft":{
         "address":"0x4961db588dd962abb20927aa38fa33e5225b3be2",
         "token_id":2928,
         "name":"2928",
         "description":null,
         "external_url":"https://stm-public.sfo3.cdn.digitaloceanspaces.com/metadata/2928",
         "original_image":"https://stm-public.sfo3.cdn.digitaloceanspaces.com/images/2928.png",
         "image":"https://media.niftyapi.xyz/0x4961db588dd962abb20927aa38fa33e5225b3be2/2928",
         "original_animation":null,
         "attributes":{
            "Body":"Bulletproof vest",
            "Eyes":"Heart glasses",
            "Head":"Police",
            "Skin":"Basic (green)",
            "Mouth":"Lip ring",
            "Background":"Turquoise"
         },
         "metadata_type":1,
         "image_type":1,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T02:37:08.930622",
         "updated_at":"2022-04-01T09:29:09.400546",
         "latest_block_number":13055547,
         "latest_log_index":416
      },
      "collection":{
         "address":"0x4961db588dd962abb20927aa38fa33e5225b3be2",
         "name":"Save the Martians",
         "symbol":"STM",
         "default_image":"https://media.niftyapi.xyz/0x4961db588dd962abb20927aa38fa33e5225b3be2/11850",
         "slug":"save-the-martians",
         "decimals":1,
         "first_block_seen":14002412,
         "type":721,
         "owner":"0xe69ccc059fe88d1e29dba68a2c4a12d72bc99ff4",
         "created_at":"2022-01-14T07:52:37.025443",
         "nft_data_base_url":"https://stm-public.sfo3.cdn.digitaloceanspaces.com/metadata/__TOKENID__",
         "nft_image_base_url":"https://stm-public.sfo3.cdn.digitaloceanspaces.com/images/__TOKENID__.png",
         "transfers_total":27920,
         "metadata":{
            "website":"https://www.savethemartians.com/",
            "image_url":"https://lh3.googleusercontent.com/hzC7cNIaqCm06O59aTi0S0VE9J5hdG_f9iKeDa0yNYVGIbrCplq5v1btXADmK71y-sG8tf0FvwIqo7umn3FwQ9NRBgnT_PTBPo7rmQ=s120",
            "description":"15,000 Martians are being forced off their home planet by Eamon Tusk’s ruthless gang of colonizing technocrats. Their only hope of survival is to travel back in time to 2021 and have themselves minted as NFTs on the blockchain by martian-loving humans.\n\nMerged collection: https://opensea.io/collection/save-the-martians-merged",
            "discord_url":"https://discord.gg/G8vS8e5BWS",
            "banner_image_url":"https://lh3.googleusercontent.com/MbM6N2GK9OD9YJEtGojZwuOq9c7M79PYvXi_CBYdhSl0ChqXp2SD9ULixNU-naB92Y_VsZNnKPsxldGXBWtg7n1jUG5JVDdRvGNchw=s2500",
            "twitter_username":"SaveMartiansNFT"
         },
         "first_transfer":"2021-08-06T23:11:13"
      }
   },
   {
      "type":"ask",
      "status":"AskCanceled",
      "block_number":"14360194",
      "log_index":"446",
      "timestamp":"2022-03-10T16:35:45.000Z",
      "transaction_hash":"0xac4a90f891c7f2a5084cc3e0ca85b91dacb04fb35378968b45ed0d3ce1b57a0e",
      "address":"0x4961db588dd962abb20927aa38fa33e5225b3be2",
      "token_id":"2928",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"100000000000000000000",
      "nft":{
         "address":"0x4961db588dd962abb20927aa38fa33e5225b3be2",
         "token_id":2928,
         "name":"2928",
         "description":null,
         "external_url":"https://stm-public.sfo3.cdn.digitaloceanspaces.com/metadata/2928",
         "original_image":"https://stm-public.sfo3.cdn.digitaloceanspaces.com/images/2928.png",
         "image":"https://media.niftyapi.xyz/0x4961db588dd962abb20927aa38fa33e5225b3be2/2928",
         "original_animation":null,
         "attributes":{
            "Body":"Bulletproof vest",
            "Eyes":"Heart glasses",
            "Head":"Police",
            "Skin":"Basic (green)",
            "Mouth":"Lip ring",
            "Background":"Turquoise"
         },
         "metadata_type":1,
         "image_type":1,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T02:37:08.930622",
         "updated_at":"2022-04-01T09:29:09.400546",
         "latest_block_number":13055547,
         "latest_log_index":416
      },
      "collection":{
         "address":"0x4961db588dd962abb20927aa38fa33e5225b3be2",
         "name":"Save the Martians",
         "symbol":"STM",
         "default_image":"https://media.niftyapi.xyz/0x4961db588dd962abb20927aa38fa33e5225b3be2/11850",
         "slug":"save-the-martians",
         "decimals":1,
         "first_block_seen":14002412,
         "type":721,
         "owner":"0xe69ccc059fe88d1e29dba68a2c4a12d72bc99ff4",
         "created_at":"2022-01-14T07:52:37.025443",
         "nft_data_base_url":"https://stm-public.sfo3.cdn.digitaloceanspaces.com/metadata/__TOKENID__",
         "nft_image_base_url":"https://stm-public.sfo3.cdn.digitaloceanspaces.com/images/__TOKENID__.png",
         "transfers_total":27920,
         "metadata":{
            "website":"https://www.savethemartians.com/",
            "image_url":"https://lh3.googleusercontent.com/hzC7cNIaqCm06O59aTi0S0VE9J5hdG_f9iKeDa0yNYVGIbrCplq5v1btXADmK71y-sG8tf0FvwIqo7umn3FwQ9NRBgnT_PTBPo7rmQ=s120",
            "description":"15,000 Martians are being forced off their home planet by Eamon Tusk’s ruthless gang of colonizing technocrats. Their only hope of survival is to travel back in time to 2021 and have themselves minted as NFTs on the blockchain by martian-loving humans.\n\nMerged collection: https://opensea.io/collection/save-the-martians-merged",
            "discord_url":"https://discord.gg/G8vS8e5BWS",
            "banner_image_url":"https://lh3.googleusercontent.com/MbM6N2GK9OD9YJEtGojZwuOq9c7M79PYvXi_CBYdhSl0ChqXp2SD9ULixNU-naB92Y_VsZNnKPsxldGXBWtg7n1jUG5JVDdRvGNchw=s2500",
            "twitter_username":"SaveMartiansNFT"
         },
         "first_transfer":"2021-08-06T23:11:13"
      }
   },
   {
      "type":"ask",
      "status":"AskCreatedOrUpdated",
      "block_number":"14360105",
      "log_index":"212",
      "timestamp":"2022-03-10T16:17:31.000Z",
      "transaction_hash":"0xbfff971c856b88f434e2628b16cef78cc463bda6a23a8e0faf545797eba710a8",
      "address":"0x4961db588dd962abb20927aa38fa33e5225b3be2",
      "token_id":"2928",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"100000000000000000000",
      "nft":{
         "address":"0x4961db588dd962abb20927aa38fa33e5225b3be2",
         "token_id":2928,
         "name":"2928",
         "description":null,
         "external_url":"https://stm-public.sfo3.cdn.digitaloceanspaces.com/metadata/2928",
         "original_image":"https://stm-public.sfo3.cdn.digitaloceanspaces.com/images/2928.png",
         "image":"https://media.niftyapi.xyz/0x4961db588dd962abb20927aa38fa33e5225b3be2/2928",
         "original_animation":null,
         "attributes":{
            "Body":"Bulletproof vest",
            "Eyes":"Heart glasses",
            "Head":"Police",
            "Skin":"Basic (green)",
            "Mouth":"Lip ring",
            "Background":"Turquoise"
         },
         "metadata_type":1,
         "image_type":1,
         "owner":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
         "created_at":"2022-01-25T02:37:08.930622",
         "updated_at":"2022-04-01T09:29:09.400546",
         "latest_block_number":13055547,
         "latest_log_index":416
      },
      "collection":{
         "address":"0x4961db588dd962abb20927aa38fa33e5225b3be2",
         "name":"Save the Martians",
         "symbol":"STM",
         "default_image":"https://media.niftyapi.xyz/0x4961db588dd962abb20927aa38fa33e5225b3be2/11850",
         "slug":"save-the-martians",
         "decimals":1,
         "first_block_seen":14002412,
         "type":721,
         "owner":"0xe69ccc059fe88d1e29dba68a2c4a12d72bc99ff4",
         "created_at":"2022-01-14T07:52:37.025443",
         "nft_data_base_url":"https://stm-public.sfo3.cdn.digitaloceanspaces.com/metadata/__TOKENID__",
         "nft_image_base_url":"https://stm-public.sfo3.cdn.digitaloceanspaces.com/images/__TOKENID__.png",
         "transfers_total":27920,
         "metadata":{
            "website":"https://www.savethemartians.com/",
            "image_url":"https://lh3.googleusercontent.com/hzC7cNIaqCm06O59aTi0S0VE9J5hdG_f9iKeDa0yNYVGIbrCplq5v1btXADmK71y-sG8tf0FvwIqo7umn3FwQ9NRBgnT_PTBPo7rmQ=s120",
            "description":"15,000 Martians are being forced off their home planet by Eamon Tusk’s ruthless gang of colonizing technocrats. Their only hope of survival is to travel back in time to 2021 and have themselves minted as NFTs on the blockchain by martian-loving humans.\n\nMerged collection: https://opensea.io/collection/save-the-martians-merged",
            "discord_url":"https://discord.gg/G8vS8e5BWS",
            "banner_image_url":"https://lh3.googleusercontent.com/MbM6N2GK9OD9YJEtGojZwuOq9c7M79PYvXi_CBYdhSl0ChqXp2SD9ULixNU-naB92Y_VsZNnKPsxldGXBWtg7n1jUG5JVDdRvGNchw=s2500",
            "twitter_username":"SaveMartiansNFT"
         },
         "first_transfer":"2021-08-06T23:11:13"
      }
   }
]
```

This endpoint returns all zora activiy for user address

### HTTP Request

`GET https://api.niftyapi.xyz/zora/activity/address/:address`

### URL Parameters
| Parameter | Description                                |
| --------- | ------------------------------------------ |
| address   | The user address to retrieve activity from |


## Get all activity for collection

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/zora/activity/collection/0x0144b7e66993c6bfab85581e8601f96bfe50c9df"
);
```

```json
[
   {
      "type":"offer",
      "status":"OfferCreatedOrUpdated",
      "block_number":"14450575",
      "log_index":"478",
      "timestamp":"2022-03-24T18:24:00.000Z",
      "transaction_hash":"0x7802a9e6c815b04ec5f23ee0c10ff89526e75799b069ab98b01060981840db2a",
      "address":"0x0144b7e66993c6bfab85581e8601f96bfe50c9df",
      "token_id":"3660",
      "seller":"0x4b5922abf25858d012d12bb1184e5d3d0b6d6be4",
      "buyer":null,
      "finder":null,
      "currency":null,
      "price":"1000000000000000",
      "nft":{
         "address":"0x0144b7e66993c6bfab85581e8601f96bfe50c9df",
         "token_id":3660,
         "name":"Pride Punk #3660",
         "description":"The first Punk Derivative",
         "external_url":"https://gateway.ipfs.io/ipfs/bafybeihuwyzyxmghhgbk5jvu4rjzwworbnvkfh6ba4pm3xrxb6iovnguhq/3660",
         "original_image":"https://gateway.ipfs.io/ipfs/bafkreieybuanpguxvashei3e2qk5throlefsboazvr6joc2cblwmqemuwy",
         "image":"https://media.niftyapi.xyz/0x0144b7e66993c6bfab85581e8601f96bfe50c9df/3660",
         "original_animation":null,
         "attributes":{
            "type":"Male",
            "accessory":"2 attributes"
         },
         "metadata_type":5,
         "image_type":4,
         "owner":"0xca72b32a2ec25eae54db599714cac0175bbccba5",
         "created_at":"2022-03-24T00:49:50.24816",
         "updated_at":"2022-04-10T13:06:28.184697",
         "latest_block_number":14558105,
         "latest_log_index":278
      },
      "collection":{
         "address":"0x0144b7e66993c6bfab85581e8601f96bfe50c9df",
         "name":"PridePunks 2018",
         "symbol":"MP",
         "default_image":"https://media.niftyapi.xyz/0x0144b7e66993c6bfab85581e8601f96bfe50c9df/0",
         "slug":"pridepunks2018",
         "decimals":1,
         "first_block_seen":14303869,
         "type":721,
         "owner":"0xe8d848debb3a3e12aa815b15900c8e020b863f31",
         "created_at":"2022-03-01T22:34:09.471895",
         "nft_data_base_url":"https://ipfs.io/ipfs/bafybeigmfmrekuq65vhsiypvmdj3zhxwa2w7jic2z7dx4vrggqj2o6cuhq/__TOKENID__",
         "nft_image_base_url":null,
         "transfers_total":27884,
         "metadata":{
            "website":"http://pridepunk.xyz",
            "image_url":"https://lh3.googleusercontent.com/DWKOSDqHY5BpP9lnXTn2Cmb5OEwzvVT01nZNwSxwzA8qXaLuagOXVaszkMcxXe6BNIGlx8CdKMzhPahwm6x21NX2p-LbsmBGBGqQ=s120",
            "description":"The FIRST CryptoPunks Derivative, in 2018!\r\n\r\n\r\nProof: (LarvaLabs Discord Announcement) https://discord.com/channels/329381334701178885/329381334701178885/460157631437340693\r\nProof: (2018 Smart Contract) https://etherscan.io/address/0x0144b7e66993c6bfab85581e8601f96bfe50c9df#code\r\n\r\nCreated as a statement on diversity in Web3, now a legitimate historical NFT.",
            "discord_url":"https://discord.gg/mnYJKxMgaU",
            "banner_image_url":"https://lh3.googleusercontent.com/weuzocbwyBu_vFwZ5BilZ7cjbk0ZPEfLCkZSE7AAO_5-q43WRgcxRQhq9gE6IvtANDXkjfI5-BInomGH8yWa_6btVCJVzGUZJaTgjQ=s2500",
            "featured_image_url":"https://lh3.googleusercontent.com/rQWHSLfzLM2HerdgsxDKBXt-NoeZbz3YOsvChohAXXooT__NmQMpgM1O2cI1EJguQUcYtV4DNpAlVxKTu3O-7S6PAJw3a6pnq0ke=s300"
         },
         "first_transfer":"2022-03-01T22:32:54"
      }
   }
]
```

This endpoint returns all zora activiy for collection

### HTTP Request

`GET https://api.niftyapi.xyz/zora/activity/collection/:collection`

### URL Parameters
| Parameter | Description                                |
| --------- | ------------------------------------------ |
| collection  | Collection address to retrieve activity from |
