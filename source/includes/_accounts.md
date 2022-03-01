# Accounts

## Get All NFTs owned by an account

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/address/0x3612b2e93b49f6c797066ca8c38b7f522b32c7cb/"
);
```

> The above command returns JSON structured like this:

```json
[
  {
    "address": "0x8a939fd297fab7388d6e6c634eee3c863626be57",
    "token_id": "17600020441",
    "name": "Afterburn #441/870",
    "description": "Afterburn by XCOPY",
    "external_url": "https://niftygateway.com/#/",
    "original_image": "https://res.cloudinary.com/nifty-gateway/image/upload/v1616442657/Ashley/Xcopy5/AFTERBURN_RED_-_XCOPY_2089_lkfib4.gif",
    "image": "https://d3nt5b5e09uon7.cloudfront.net/0x8a939fd297fab7388d6e6c634eee3c863626be57/17600020441",
    "original_animation": null,
    "attributes": null,
    "metadata_type": 1,
    "image_type": 1,
    "owner": "0x3612b2e93b49f6c797066ca8c38b7f522b32c7cb",
    "created_at": "2022-01-05T01:34:28.873Z",
    "updated_at": "2022-01-05T02:05:33.351Z",
    "latest_block_number": "13942539",
    "latest_log_index": "0",
    "search_weights": "'441/870':2A 'afterburn':1A,3B 'xcopi':5B"
  },
  ...
]
```

This endpoint retrieves all NFTs owned by an account.

### HTTP Request

`GET https://api.niftyapi.xyz/address/:address/`

### URL Parameters

| Parameter | Description                            |
| --------- | -------------------------------------- |
| Address   | The Address of the account to retrieve |

### Query Parameters

| Parameter  | Default | Description                     |
| ---------- | ------- | ------------------------------- |
| collection |         | Filter by collection address    |
| perPage    | 20      | Number of collections to return |
| page       | 0       | The page (for pagination)       |



## Get All NFTs owned by an account

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/address/0x3612b2e93b49f6c797066ca8c38b7f522b32c7cb/"
);
```

> The above command returns JSON structured like this:

```json
[
  {
    "collection": "0x90d4ffbf13bf3203940e6dace392f7c23ff6b9ed",
    "block_number": "14291770",
    "transaction_hash": "0x3df418e94e3fdc901f429113edb1366df63c2a43068e9460ea03dda2c663564d",
    "transaction_index": "120",
    "tx_to": "0x90d4ffbf13bf3203940e6dace392f7c23ff6b9ed",
    "tx_from": "0x047f606fd5b2baa5f5c6c4ab8958e45cb6b054b7",
    "log_index": "285",
    "transfer_index": "0",
    "timestamp": "2022-02-28T01:44:44.000Z",
    "to": "0x047f606fd5b2baa5f5c6c4ab8958e45cb6b054b7",
    "from": "0x047f606fd5b2baa5f5c6c4ab8958e45cb6b054b7",
    "amount": "1",
    "token_id": "8296",
    "gas_price": "53380609957",
    "created_at": "2022-02-25T19:15:35.057Z",
    "address": "0x90d4ffbf13bf3203940e6dace392f7c23ff6b9ed",
    "name": "Cupcat Kitten 8296",
    "description": "Cupcat Kittens are a collection made by Cupcats as 2nd season. This collection includes cute kittens that are part of Cupcats ecosystem.",
    "external_url": "https://gateway.ipfs.io/ipfs/QmZKXExwT5AMyr3MHQ4HJoBabaXfjEXKLtocnUFXHZ6GPU/8296.json",
    "original_image": "https://gateway.ipfs.io/ipfs/Qme9wQdbzn88126BR6fGtR8RW7x5EcDQwJUnuwADVRLj62",
    "image": "https://gateway.ipfs.io/ipfs/Qme9wQdbzn88126BR6fGtR8RW7x5EcDQwJUnuwADVRLj62",
    "original_animation": null,
    "attributes": null,
    "metadata_type": 5,
    "image_type": 0,
    "owner": "0x047f606fd5b2baa5f5c6c4ab8958e45cb6b054b7",
    "updated_at": "2022-02-28T01:47:12.343Z",
    "latest_block_number": "14291770",
    "latest_log_index": "285",
    "search_weights": "'2nd':13B '8296':3A 'collect':8B,16B 'cupcat':1A,4B,11B,24B 'cute':18B 'ecosystem':25B 'includ':17B 'kitten':2A,5B,19B 'made':9B 'part':22B 'season':14B"
  },
  ...
]
```

This endpoint retrieves all NFTs transfers related to an address (received or sent).

### HTTP Request

`GET https://api.niftyapi.xyz/address/:address/activity`

### URL Parameters

| Parameter | Description                            |
| --------- | -------------------------------------- |
| Address   | The Address of the account to retrieve |


