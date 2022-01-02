# Collections

## Get All Collections

```javascript
const axios = require("axios");

let { data: collections } = await axios(
  "https://nft-data.vercel.app/collections"
);
```

> The above command returns JSON structured like this:

```json
[
  {
    "address": "0x0e4b8e24789630618aa90072f520711d3d9db647",
    "name": "Flipmap",
    "symbol": "FLIP",
    "default_image": "https://d3nt5b5e09uon7.cloudfront.net/0x0e4b8e24789630618aa90072f520711d3d9db647/1700",
    "slug": "flipmap",
    "decimals": "1",
    "first_block_seen": "13920922",
    "type": 721,
    "owner": "0x0000000000000000000000000000000000000000",
    "created_at": "2022-01-01T17:41:04.864Z",
    "nft_data_base_url": null,
    "nft_image_base_url": null,
    "search_weights": "'flip':2B 'flipmap':1A,3C",
    "transfers_total": "10362",
    "transfers_hour": "9308",
    "transfers_today": "10362",
    "transfers_week": "10362",
    "receivers_total": "3680",
    "receivers_hour": "3680",
    "receivers_today": "3680",
    "receivers_week": "3680",
    "mints_hour": "7259",
    "mints_today": "8300",
    "mints_week": "8300",
    "supply": "8300",
    "owners": "3048"
  },
  {
    "address": "0x280f2599693159a96e367b621670840fcff06ee2",
    "name": "CosmicMice",
    "symbol": "CM",
    "default_image": "https://d3nt5b5e09uon7.cloudfront.net/0x280f2599693159a96e367b621670840fcff06ee2/2",
    "slug": "cosmicmice",
    "decimals": "1",
    "first_block_seen": "13922596",
    "type": 721,
    "owner": "0x2841f909a115b63a97816f52bf69b828a4577d07",
    "created_at": "2022-01-01T23:45:49.220Z",
    "nft_data_base_url": "ipfs://Qmc82EjDTo1uF5Uvse5GzQm49Ac7Mw2wuztrnP5ggScVFk/__TOKENID__.json",
    "nft_image_base_url": "ipfs://QmVqeR36ZvXju74Eq7xRBdgwmUxRWTLCDTx4iZd9eFABY6/__TOKENID__.png",
    "search_weights": "'cm':2B 'cosmicmic':1A,3C",
    "transfers_total": "7535",
    "transfers_hour": "7535",
    "transfers_today": "7535",
    "transfers_week": "7535",
    "receivers_total": "1370",
    "receivers_hour": "1370",
    "receivers_today": "1370",
    "receivers_week": "1370",
    "mints_hour": "6666",
    "mints_today": "6666",
    "mints_week": "6666",
    "supply": "6666",
    "owners": "1265"
  }
]
```

This endpoint retrieves all collections.

### HTTP Request

`GET https://nft-data.vercel.app/collections`

### Query Parameters

| Parameter | Default | Description                     |
| --------- | ------- | ------------------------------- |
| perPage   | 10      | Number of collections to return |
| page      | 0       | The page (for pagination)       |

<!-- <aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside> -->

## Get a Specific colletction

```javascript
const axios = require("axios");

let { data: collection } = await axios(
  "https://nft-data.vercel.app/collection/:address/"
);
```

> The above command returns JSON structured like this:

```json
[
  {
    "address": "0x0e4b8e24789630618aa90072f520711d3d9db647",
    "name": "Flipmap",
    "symbol": "FLIP",
    "default_image": "https://d3nt5b5e09uon7.cloudfront.net/0x0e4b8e24789630618aa90072f520711d3d9db647/1700",
    "slug": "flipmap",
    "decimals": "1",
    "first_block_seen": "13920922",
    "type": 721,
    "owner": "0x0000000000000000000000000000000000000000",
    "created_at": "2022-01-01T17:41:04.864Z",
    "nft_data_base_url": null,
    "nft_image_base_url": null,
    "search_weights": "'flip':2B 'flipmap':1A,3C",
    "transfers_total": "11043",
    "transfers_hour": "9989",
    "transfers_today": "11043",
    "transfers_week": "11043",
    "receivers_total": "4010",
    "receivers_hour": "4010",
    "receivers_today": "4010",
    "receivers_week": "4010",
    "mints_hour": "7259",
    "mints_today": "8300",
    "mints_week": "8300",
    "supply": "8300",
    "owners": "3153"
  },
  {
    "address": "0x280f2599693159a96e367b621670840fcff06ee2",
    "name": "CosmicMice",
    "symbol": "CM",
    "default_image": "https://d3nt5b5e09uon7.cloudfront.net/0x280f2599693159a96e367b621670840fcff06ee2/2",
    "slug": "cosmicmice",
    "decimals": "1",
    "first_block_seen": "13922596",
    "type": 721,
    "owner": "0x2841f909a115b63a97816f52bf69b828a4577d07",
    "created_at": "2022-01-01T23:45:49.220Z",
    "nft_data_base_url": "ipfs://Qmc82EjDTo1uF5Uvse5GzQm49Ac7Mw2wuztrnP5ggScVFk/__TOKENID__.json",
    "nft_image_base_url": "ipfs://QmVqeR36ZvXju74Eq7xRBdgwmUxRWTLCDTx4iZd9eFABY6/__TOKENID__.png",
    "search_weights": "'cm':2B 'cosmicmic':1A,3C",
    "transfers_total": "7632",
    "transfers_hour": "7632",
    "transfers_today": "7632",
    "transfers_week": "7632",
    "receivers_total": "1394",
    "receivers_hour": "1394",
    "receivers_today": "1394",
    "receivers_week": "1394",
    "mints_hour": "6666",
    "mints_today": "6666",
    "mints_week": "6666",
    "supply": "6666",
    "owners": "1286"
  }
]
```

This endpoint retrieves a specific collection.

<!-- <aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside> -->

### HTTP Request

`GET https://nft-data.vercel.app/collection/:address/`

### URL Parameters

| Parameter | Description                               |
| --------- | ----------------------------------------- |
| Address   | The Address of the collection to retrieve |
