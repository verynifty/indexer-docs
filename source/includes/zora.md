# Zora Marketplace Data

##  Get all active Asks for owner

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
| token_id   | the token id for NFT |

## Ask for Collection

https://api.niftyapi.xyz/zora/ask/collection/:collection

## Offer for owner

https://api.niftyapi.xyz/zora/offers/owner/:address

## Offer for NFT

https://api.niftyapi.xyz/zora/offers/nft/:collection/:token_id

## Offer for Collection

https://api.niftyapi.xyz/zora/offers/collection/:collection

## Activity for Address

https://api.niftyapi.xyz/zora/activity/address/:address

## Activity for Collection

https://api.niftyapi.xyz/zora/activity/collection/:collection
