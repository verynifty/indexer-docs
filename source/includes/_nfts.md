# NFTs

## Get All NFTs in a collection

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/collection/nfts/0xc3f733ca98e0dad0386979eb96fb1722a1a05e69"
);
```

> The above command returns JSON structured like this:

```json
[
  {
    "address": "0x0e4b8e24789630618aa90072f520711d3d9db647",
    "token_id": "8882",
    "name": "#8882 - Processing Hand",
    "description": "Flipmaps are the lost 8,300 Blitmaps, only flipped.",
    "external_url": null,
    "original_image": null,
    "image": "https://d3nt5b5e09uon7.cloudfront.net/0x0e4b8e24789630618aa90072f520711d3d9db647/8882",
    "original_animation": null,
    "attributes": "\"Type\"=>\"Flipling\", \"Slabs\"=>\"◣ ◤ ◣ ◣\", \"Palette\"=>\"Hand (#57)\", \"Affinity\"=>\"Fire III\", \"Composition\"=>\"Processing (#22)\"",
    "metadata_type": 3,
    "image_type": 2,
    "owner": "0x3e528ad9f3975f247243336d28596be4965b3c59",
    "created_at": "2022-01-02T02:43:41.586Z",
    "updated_at": "2022-01-02T12:57:23.057Z",
    "latest_block_number": "13926089",
    "latest_log_index": "64",
    "search_weights": "'300':9B '8':8B '8882':1A 'blitmap':10B 'flip':12B 'flipmap':4B 'hand':3A 'lost':7B 'process':2A"
  }
]
```

This endpoint retrieves all NFTs in a collection.

### HTTP Request

`GET https://api.niftyapi.xyz/collection/nfts/:address`

### URL Parameters

| Parameter | Description                          |
| --------- | ------------------------------------ |
| Address   | The collection to retrieve NFTs from |

## Get a specific NFT

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/nft/0xc3f733ca98e0dad0386979eb96fb1722a1a05e69/7120"
);
```

> The above command returns JSON structured like this:

```json
[
  {
    "address": "0x0e4b8e24789630618aa90072f520711d3d9db647",
    "token_id": "5546",
    "name": "#5546 - Overloaded Cloudy",
    "description": "Flipmaps are the lost 8,300 Blitmaps, only flipped.",
    "external_url": null,
    "original_image": null,
    "image": "https://d3nt5b5e09uon7.cloudfront.net/0x0e4b8e24789630618aa90072f520711d3d9db647/5546",
    "original_animation": null,
    "attributes": "\"Type\"=>\"Flipling\", \"Slabs\"=>\"◥ ◢ ◢ ◢\", \"Palette\"=>\"Cloudy (#34)\", \"Affinity\"=>\"Water I, Fire I, Earth I\", \"Composition\"=>\"Overloaded (#14)\"",
    "metadata_type": 3,
    "image_type": 2,
    "owner": "0x1dee8aef0c3b6b90748f970d9e092d1a50f3715a",
    "created_at": "2022-01-02T02:10:07.026Z",
    "updated_at": "2022-01-02T12:19:10.619Z",
    "latest_block_number": "13925914",
    "latest_log_index": "458",
    "search_weights": "'300':9B '5546':1A '8':8B 'blitmap':10B 'cloudi':3A 'flip':12B 'flipmap':4B 'lost':7B 'overload':2A"
  }
]
```

This endpoint retrieves a single NFT in a collection.

### HTTP Request

`GET https://api.niftyapi.xyz/nft/:address/:id/`

### URL Parameters

| Parameter | Description                          |
| --------- | ------------------------------------ |
| Address   | The collection to retrieve NFTs from |
| ID        | The NFT ID To retrieve               |

## Get trading history for Specific NFT

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/transfers/0xc3f733ca98e0dad0386979eb96fb1722a1a05e69/7120"
);
```

> The above command returns JSON structured like this:

```json
[
  {
    "collection": "0x0e4b8e24789630618aa90072f520711d3d9db647",
    "block_number": "13925925",
    "transaction_hash": "0x6449e72d3fa5f186899d24ed94c5c78408dcdd6f8e4ad6be177b21c68f4a3a3e",
    "transaction_index": "213",
    "tx_to": "0x7be8076f4ea4a4ad08075c2508e481d6c946d12b",
    "tx_from": "0x3d8d744f2bfdd1d36638a625992f4d7aebee878a",
    "log_index": "501",
    "transfer_index": "0",
    "timestamp": "2022-01-02T12:20:19.000Z",
    "to": "0x3d8d744f2bfdd1d36638a625992f4d7aebee878a",
    "from": "0x809fd9c429ba301da0873879bd28c6809334a00a",
    "amount": "1",
    "token_id": "4755",
    "gas_price": "72750706989",
    "created_at": "2022-01-02T01:56:19.779Z",
    "address": "0x0e4b8e24789630618aa90072f520711d3d9db647",
    "name": "#4755 - Totally Dunce",
    "description": "Flipmaps are the lost 8,300 Blitmaps, only flipped.",
    "external_url": null,
    "original_image": null,
    "image": "https://d3nt5b5e09uon7.cloudfront.net/0x0e4b8e24789630618aa90072f520711d3d9db647/4755",
    "original_animation": null,
    "attributes": "\"Type\"=>\"Flipling\", \"Slabs\"=>\"◣ ◢ ◢ ◢\", \"Palette\"=>\"Dunce (#68)\", \"Affinity\"=>\"Fire III\", \"Composition\"=>\"Totally (#9)\"",
    "metadata_type": 3,
    "image_type": 2,
    "owner": "0x3d8d744f2bfdd1d36638a625992f4d7aebee878a",
    "updated_at": "2022-01-02T12:21:11.331Z",
    "latest_block_number": "13925925",
    "latest_log_index": "501",
    "search_weights": "'300':9B '4755':1A '8':8B 'blitmap':10B 'dunc':3A 'flip':12B 'flipmap':4B 'lost':7B 'total':2A"
  }
]
```

This endpoint retrieves transfer history of a single NFT.

### HTTP Request

`GET https://api.niftyapi.xyz/transfers/:address/:id`

### URL Parameters

| Parameter | Description                         |
| --------- | ----------------------------------- |
| Address   | The NFT collection to retrieve from |
| ID        | The NFT ID To retrieve              |
