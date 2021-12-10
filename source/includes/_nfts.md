# NFTs

## Get All NFTs in a collection

```javascript
const axios = require("axios");

let { data: nfts } = await axios("api");
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves all NFTs in a collection.

### HTTP Request

`GET http://example.com/collection/nfts/:address/`

### URL Parameters

| Parameter | Description                          |
| --------- | ------------------------------------ |
| Address   | The collection to retrieve NFTs from |

## Get a specific NFT

```javascript
const axios = require("axios");

let { data: nfts } = await axios("api");
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves a single NFT in a collection.

### HTTP Request

`GET http://example.com/nft/:address/:id/`

### URL Parameters

| Parameter | Description                          |
| --------- | ------------------------------------ |
| Address   | The collection to retrieve NFTs from |
| ID        | The NFT ID To retrieve               |
