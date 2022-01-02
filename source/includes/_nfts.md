# NFTs

## Get All NFTs in a collection

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://nft-data.vercel.app/collection/nfts/:address"
);
```

> The above command returns JSON structured like this:

```json
[
  {
    "address":"0x0e4b8e24789630618aa90072f520711d3d9db647",
    "token_id":"8882",
    "name":"#8882 - Processing Hand",
    "description":"Flipmaps are the lost 8,300 Blitmaps, only flipped.",
    "external_url":null,
    "original_image":null,
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x0e4b8e24789630618aa90072f520711d3d9db647/8882",
    "original_animation":null,
    "attributes":"\"Type\"=>\"Flipling\", \"Slabs\"=>\"◣ ◤ ◣ ◣\", \"Palette\"=>\"Hand (#57)\", \"Affinity\"=>\"Fire III\", \"Composition\"=>\"Processing (#22)\"",
    "metadata_type":3,
    "image_type":2,
    "owner":"0x3e528ad9f3975f247243336d28596be4965b3c59",
    "created_at":"2022-01-02T02:43:41.586Z",
    "updated_at":"2022-01-02T12:57:23.057Z",
    "latest_block_number":"13926089",
    "latest_log_index":"64",
    "search_weights":"'300':9B '8':8B '8882':1A 'blitmap':10B 'flip':12B 'flipmap':4B 'hand':3A 'lost':7B 'process':2A"
  },
  {
    "address":"0x0e4b8e24789630618aa90072f520711d3d9db647",
    "token_id":"3656",
    "name":"#3656 - Genesis Swordy",
    "description":"Flipmaps are the lost 8,300 Blitmaps, only flipped.",
    "external_url":null,
    "original_image":null,
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x0e4b8e24789630618aa90072f520711d3d9db647/3656",
    "original_animation":null,
    "attributes":"\"Type\"=>\"Flipling\", \"Slabs\"=>\"◥ ◤ ◣ ◤\", \"Palette\"=>\"Swordy (#29)\", \"Affinity\"=>\"Fire III\", \"Composition\"=>\"Genesis (#0)\"",
    "metadata_type":3,
    "image_type":2,
    "owner":"0x220ee648ebe5bb4fe52cb24898d51e4449efa42b",
    "created_at":"2022-01-02T01:10:28.386Z",
    "updated_at":"2022-01-02T12:56:30.723Z",
    "latest_block_number":"13926086",
    "latest_log_index":"125",
    "search_weights":"'300':9B '3656':1A '8':8B 'blitmap':10B 'flip':12B 'flipmap':4B 'genesi':2A 'lost':7B 'swordi':3A"
  },
  {
    "address":"0x280f2599693159a96e367b621670840fcff06ee2",
    "token_id":"4747",
    "name":"Cosmic Mice #4747",
    "description":"Races of mice fight together in this degen friendly PvP experiment",
    "external_url":null,
    "original_image":"ipfs://QmVqeR36ZvXju74Eq7xRBdgwmUxRWTLCDTx4iZd9eFABY6/4747.png",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x280f2599693159a96e367b621670840fcff06ee2/4747",
    "original_animation":null,
    "attributes":"\"Ears\"=>\"Stud Left\", \"Eyes\"=>\"Glasses Green\", \"Face\"=>\"Assorted\", \"Head\"=>\"Neon Blue\", \"Nose\"=>\"Normal\", \"Race\"=>\"Alien\", \"Mouth\"=>\"Mask Gray\", \"Power\"=>\"6\", \"Collar\"=>\"Blue\", \"Background\"=>\"Green\"",
    "metadata_type":5,
    "image_type":4,
    "owner":"0x04ebe8ab7b47795f96a5f5542801aba4d598f458",
    "created_at":"2022-01-02T01:26:57.860Z",
    "updated_at":"2022-01-02T13:58:55.359Z",
    "latest_block_number":"13926384",
    "latest_log_index":"328",
    "search_weights":"'4747':3A 'cosmic':1A 'degen':11B 'experi':14B 'fight':7B 'friend':12B 'mice':2A,6B 'pvp':13B 'race':4B 'togeth':8B"
  },
  {
    "address":"0x280f2599693159a96e367b621670840fcff06ee2",
    "token_id":"3230",
    "name":"Cosmic Mice #3230",
    "description":"Races of mice fight together in this degen friendly PvP experiment",
    "external_url":null,
    "original_image":"ipfs://QmVqeR36ZvXju74Eq7xRBdgwmUxRWTLCDTx4iZd9eFABY6/3230.png",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x280f2599693159a96e367b621670840fcff06ee2/3230",
    "original_animation":null,
    "attributes":"\"Ears\"=>\"Tag Right\", \"Eyes\"=>\"Brows Green\", \"Face\"=>\"Glow Red\", \"Head\"=>\"Neon Green\", \"Nose\"=>\"Normal\", \"Race\"=>\"Alien\", \"Mouth\"=>\"Mask Purple\", \"Power\"=>\"7\", \"Collar\"=>\"None\", \"Background\"=>\"Purple\"",
    "metadata_type":5,
    "image_type":4,
    "owner":"0xc9ea196c466b87fc4dc49f8c27b2285f9c3d5a0c",
    "created_at":"2022-01-02T01:22:38.868Z",
    "updated_at":"2022-01-02T13:50:21.409Z",
    "latest_block_number":"13926341",
    "latest_log_index":"227",
    "search_weights":"'3230':3A 'cosmic':1A 'degen':11B 'experi':14B 'fight':7B 'friend':12B 'mice':2A,6B 'pvp':13B 'race':4B 'togeth':8B"
  }
]
```

This endpoint retrieves all NFTs in a collection.

### HTTP Request

`GET https://nft-data.vercel.app/collection/nfts/:address`

### URL Parameters

| Parameter | Description                          |
| --------- | ------------------------------------ |
| Address   | The collection to retrieve NFTs from |

## Get a specific NFT

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "http://nft-data.vercel.app/nft/:address/:id/"
);
```

> The above command returns JSON structured like this:

```json
[
  {
    "address":"0x0e4b8e24789630618aa90072f520711d3d9db647",
    "token_id":"5546",
    "name":"#5546 - Overloaded Cloudy",
    "description":"Flipmaps are the lost 8,300 Blitmaps, only flipped.",
    "external_url":null,
    "original_image":null,
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x0e4b8e24789630618aa90072f520711d3d9db647/5546",
    "original_animation":null,
    "attributes":"\"Type\"=>\"Flipling\", \"Slabs\"=>\"◥ ◢ ◢ ◢\", \"Palette\"=>\"Cloudy (#34)\", \"Affinity\"=>\"Water I, Fire I, Earth I\", \"Composition\"=>\"Overloaded (#14)\"",
    "metadata_type":3,
    "image_type":2,
    "owner":"0x1dee8aef0c3b6b90748f970d9e092d1a50f3715a",
    "created_at":"2022-01-02T02:10:07.026Z",
    "updated_at":"2022-01-02T12:19:10.619Z",
    "latest_block_number":"13925914",
    "latest_log_index":"458",
    "search_weights":"'300':9B '5546':1A '8':8B 'blitmap':10B 'cloudi':3A 'flip':12B 'flipmap':4B 'lost':7B 'overload':2A"
  },
  {
    "address":"0x0e4b8e24789630618aa90072f520711d3d9db647",
    "token_id":"4755",
    "name":"#4755 - Totally Dunce",
    "description":"Flipmaps are the lost 8,300 Blitmaps, only flipped.",
    "external_url":null,
    "original_image":null,
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x0e4b8e24789630618aa90072f520711d3d9db647/4755",
    "original_animation":null,
    "attributes":"\"Type\"=>\"Flipling\", \"Slabs\"=>\"◣ ◢ ◢ ◢\", \"Palette\"=>\"Dunce (#68)\", \"Affinity\"=>\"Fire III\", \"Composition\"=>\"Totally (#9)\"",
    "metadata_type":3,
    "image_type":2,"owner":"0x3d8d744f2bfdd1d36638a625992f4d7aebee878a",
    "created_at":"2022-01-02T01:56:19.779Z",
    "updated_at":"2022-01-02T12:21:11.331Z",
    "latest_block_number":"13925925",
    "latest_log_index":"501",
    "search_weights":"'300':9B '4755':1A '8':8B 'blitmap':10B 'dunc':3A 'flip':12B 'flipmap':4B 'lost':7B 'total':2A"
  },
  {
    "address":"0x280f2599693159a96e367b621670840fcff06ee2",
    "token_id":"2404",
    "name":"Cosmic Mice",
    "description":"Races of mice fight together in this degen friendly PvP experiment",
    "external_url":null,
    "original_image":"https://lh3.googleusercontent.com/y1Yg9XgllhAIN3yYT27PZzeOEcOXOCwp7Q6icMdBlGtSaWsEXLkOCqmATjMRLIQY8MgqDAGEoce3YrXHVzdHAkmdBuK9SpIvolvh_4c",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x280f2599693159a96e367b621670840fcff06ee2/2404",
    "original_animation":null,
    "attributes":"",
    "metadata_type":4,
    "image_type":5,
    "owner":"0x49131f1a71414cc29fe5a8d408dd6aafe0e48c4d",
    "created_at":"2022-01-02T01:20:37.232Z",
    "updated_at":"2022-01-02T11:50:24.519Z",
    "latest_block_number":"13925787",
    "latest_log_index":"429",
    "search_weights":"'cosmic':1A 'degen':10B 'experi':13B 'fight':6B 'friend':11B 'mice':2A,5B 'pvp':12B 'race':3B 'togeth':7B"
  },
  {
    "address":"0x280f2599693159a96e367b621670840fcff06ee2",
    "token_id":"2245",
    "name":"Cosmic Mice",
    "description":"Races of mice fight together in this degen friendly PvP experiment",
    "external_url":null,
    "original_image":"https://lh3.googleusercontent.com/y1Yg9XgllhAIN3yYT27PZzeOEcOXOCwp7Q6icMdBlGtSaWsEXLkOCqmATjMRLIQY8MgqDAGEoce3YrXHVzdHAkmdBuK9SpIvolvh_4c",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x280f2599693159a96e367b621670840fcff06ee2/2245",
    "original_animation":null,
    "attributes":"",
    "metadata_type":4,
    "image_type":5,
    "owner":"0x5af1c6c005ce3b0238304d022ef5fa5b240fcc55",
    "created_at":"2022-01-02T01:20:06.302Z",
    "updated_at":"2022-01-02T11:24:27.458Z",
    "latest_block_number":"13925689",
    "latest_log_index":"398",
    "search_weights":"'cosmic':1A 'degen':10B 'experi':13B 'fight':6B 'friend':11B 'mice':2A,5B 'pvp':12B 'race':3B 'togeth':7B"
  }
]
```

This endpoint retrieves a single NFT in a collection.

### HTTP Request

`GET http://nft-data.vercel.app/nft/:address/:id/`

### URL Parameters

| Parameter | Description                          |
| --------- | ------------------------------------ |
| Address   | The collection to retrieve NFTs from |
| ID        | The NFT ID To retrieve               |

## Get trading history for Specific NFT

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "http://nft-data.vercel.app/transfers/:address/:id"
);
```

> The above command returns JSON structured like this:

```json
[
  {
    "collection":"0x0e4b8e24789630618aa90072f520711d3d9db647",
    "block_number":"13925925",
    "transaction_hash":"0x6449e72d3fa5f186899d24ed94c5c78408dcdd6f8e4ad6be177b21c68f4a3a3e",
    "transaction_index":"213",
    "tx_to":"0x7be8076f4ea4a4ad08075c2508e481d6c946d12b",
    "tx_from":"0x3d8d744f2bfdd1d36638a625992f4d7aebee878a",
    "log_index":"501",
    "transfer_index":"0",
    "timestamp":"2022-01-02T12:20:19.000Z",
    "to":"0x3d8d744f2bfdd1d36638a625992f4d7aebee878a",
    "from":"0x809fd9c429ba301da0873879bd28c6809334a00a",
    "amount":"1",
    "token_id":"4755",
    "gas_price":"72750706989",
    "created_at":"2022-01-02T01:56:19.779Z",
    "address":"0x0e4b8e24789630618aa90072f520711d3d9db647",
    "name":"#4755 - Totally Dunce",
    "description":"Flipmaps are the lost 8,300 Blitmaps, only flipped.",
    "external_url":null,
    "original_image":null,
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x0e4b8e24789630618aa90072f520711d3d9db647/4755",
    "original_animation":null,
    "attributes":"\"Type\"=>\"Flipling\", \"Slabs\"=>\"◣ ◢ ◢ ◢\", \"Palette\"=>\"Dunce (#68)\", \"Affinity\"=>\"Fire III\", \"Composition\"=>\"Totally (#9)\"",
    "metadata_type":3,
    "image_type":2,
    "owner":"0x3d8d744f2bfdd1d36638a625992f4d7aebee878a",
    "updated_at":"2022-01-02T12:21:11.331Z",
    "latest_block_number":"13925925",
    "latest_log_index":"501",
    "search_weights":"'300':9B '4755':1A '8':8B 'blitmap':10B 'dunc':3A 'flip':12B 'flipmap':4B 'lost':7B 'total':2A"
  },
  {
    "collection":"0x0e4b8e24789630618aa90072f520711d3d9db647",
    "block_number":"13923191",
    "transaction_hash":"0x85ace4e6eb6b420c7edfab28aea72eaa5bef513b3484f0d14adbc4115f688de5",
    "transaction_index":"62",
    "tx_to":"0x0e4b8e24789630618aa90072f520711d3d9db647",
    "tx_from":"0x809fd9c429ba301da0873879bd28c6809334a00a",
    "log_index":"41",
    "transfer_index":"0",
    "timestamp":"2022-01-02T01:54:33.000Z",
    "to":"0x809fd9c429ba301da0873879bd28c6809334a00a",
    "from":"0x0000000000000000000000000000000000000000",
    "amount":"1",
    "token_id":"4755",
    "gas_price":"101003100285",
    "created_at":"2022-01-02T01:56:19.779Z",
    "address":"0x0e4b8e24789630618aa90072f520711d3d9db647",
    "name":"#4755 - Totally Dunce",
    "description":"Flipmaps are the lost 8,300 Blitmaps, only flipped.",
    "external_url":null,
    "original_image":null,
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x0e4b8e24789630618aa90072f520711d3d9db647/4755",
    "original_animation":null,
    "attributes":"\"Type\"=>\"Flipling\", \"Slabs\"=>\"◣ ◢ ◢ ◢\", \"Palette\"=>\"Dunce (#68)\", \"Affinity\"=>\"Fire III\", \"Composition\"=>\"Totally (#9)\"",
    "metadata_type":3,
    "image_type":2,
    "owner":"0x3d8d744f2bfdd1d36638a625992f4d7aebee878a",
    "updated_at":"2022-01-02T12:21:11.331Z",
    "latest_block_number":"13925925",
    "latest_log_index":"501",
    "search_weights":"'300':9B '4755':1A '8':8B 'blitmap':10B 'dunc':3A 'flip':12B 'flipmap':4B 'lost':7B 'total':2A"
  },
  {
    "collection":"0x280f2599693159a96e367b621670840fcff06ee2",
    "block_number":"13925857",
    "transaction_hash":"0xfdceb7f8dd26df7c115b0fc5bcdb7a63cb55a32eb39b116e6813f16f2daee26f",
    "transaction_index":"186",
    "tx_to":"0x0a267cf51ef038fc00e71801f5a524aec06e4f07",
    "tx_from":"0xf0a5043111c2a35fbd1acfb588c382e781ad6aef",
    "log_index":"207",
    "transfer_index":"0",
    "timestamp":"2022-01-02T12:02:50.000Z",
    "to":"0xf0a5043111c2a35fbd1acfb588c382e781ad6aef",
    "from":"0x72df07d6cb06d55b4e38f0b3761e0406e3fb38f6",
    "amount":"1",
    "token_id":"973",
    "gas_price":"51839405234",
    "created_at":"2022-01-02T01:13:32.938Z",
    "address":"0x280f2599693159a96e367b621670840fcff06ee2",
    "name":"Cosmic Mice",
    "description":"Races of mice fight together in this degen friendly PvP experiment",
    "external_url":null,
    "original_image":"ipfs://QmUkYRYSK4NhdF7CcrUA1F73ESDJcCiVARNHWh2QS4vLsE/hidden.gif",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x280f2599693159a96e367b621670840fcff06ee2/973",
    "original_animation":null,
    "attributes":null,
    "metadata_type":5,
    "image_type":4,
    "owner":"0xf0a5043111c2a35fbd1acfb588c382e781ad6aef",
    "updated_at":"2022-01-02T12:03:56.459Z",
    "latest_block_number":"13925857",
    "latest_log_index":"207",
    "search_weights":"'cosmic':1A 'degen':10B 'experi':13B 'fight':6B 'friend':11B 'mice':2A,5B 'pvp':12B 'race':3B 'togeth':7B"
  },
  {
    "collection":"0x280f2599693159a96e367b621670840fcff06ee2",
    "block_number":"13923004",
    "transaction_hash":"0xf7c9e1b7bc683ef08d6c63ef3bfec43373f6cb9f5798bccb6f73ae45f59c4718",
    "transaction_index":"161",
    "tx_to":"0x280f2599693159a96e367b621670840fcff06ee2",
    "tx_from":"0x72df07d6cb06d55b4e38f0b3761e0406e3fb38f6",
    "log_index":"268",
    "transfer_index":"0",
    "timestamp":"2022-01-02T01:11:21.000Z",
    "to":"0x72df07d6cb06d55b4e38f0b3761e0406e3fb38f6",
    "from":"0x0000000000000000000000000000000000000000",
    "amount":"1",
    "token_id":"973",
    "gas_price":"68811070431",
    "created_at":"2022-01-02T01:13:32.938Z",
    "address":"0x280f2599693159a96e367b621670840fcff06ee2",
    "name":"Cosmic Mice",
    "description":"Races of mice fight together in this degen friendly PvP experiment",
    "external_url":null,
    "original_image":"ipfs://QmUkYRYSK4NhdF7CcrUA1F73ESDJcCiVARNHWh2QS4vLsE/hidden.gif",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x280f2599693159a96e367b621670840fcff06ee2/973",
    "original_animation":null,
    "attributes":null,
    "metadata_type":5,
    "image_type":4,
    "owner":"0xf0a5043111c2a35fbd1acfb588c382e781ad6aef",
    "updated_at":"2022-01-02T12:03:56.459Z",
    "latest_block_number":"13925857",
    "latest_log_index":"207",
    "search_weights":"'cosmic':1A 'degen':10B 'experi':13B 'fight':6B 'friend':11B 'mice':2A,5B 'pvp':12B 'race':3B 'togeth':7B"
  }
]
```

This endpoint retrieves transfer history of a single NFT.

### HTTP Request

`GET http://nft-data.vercel.app/transfers/:address/:id`

### URL Parameters

| Parameter | Description                         |
| --------- | ----------------------------------- |
| Address   | The NFT collection to retrieve from |
| ID        | The NFT ID To retrieve              |
