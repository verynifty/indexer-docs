# Stats

## Get NFTs trading data

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://api.niftyapi.xyz/trades/collections?orderBy=volume_day&page=1&perPage=1"
);
```

> The above command returns JSON structured like this:

```json
{
    "collections": [{
        "address": "0x659a4bdaaacc62d2bd9cb18225d9c89b5b697a5a",
        "transfers_total": "30748",
        "supply": "6666",
        "owners": "3113",
        "transfers_daily": "30595",
        "receivers_daily": "12253",
        "senders_daily": "10450",
        "transfers_hourly": "3545",
        "receivers_hourly": "1698",
        "senders_hourly": "1886",
        "trades_current_day": {
            "volume": 1275.90534558,
            "trades": 811,
            "min_price": 0.699,
            "max_price": 45,
            "median_price": 1.45,
            "buyers": 589,
            "sellers": 601,
            "marketplaces": 1,
            "current_collection": "0x659a4bdaaacc62d2bd9cb18225d9c89b5b697a5a"
        },
        "trades_previous_day": {
            "volume": 1480.33511319,
            "trades": 1388,
            "min_price": 0.098,
            "max_price": 69.42,
            "median_price": 0.98,
            "buyers": 935,
            "sellers": 948,
            "marketplaces": 1,
            "previous_collection": "0x659a4bdaaacc62d2bd9cb18225d9c89b5b697a5a"
        },
        "trades_current_hour": null,
        "trades_previous_hour": null,
        "trades_current_week": {
            "volume": 8589.716710128467,
            "trades": 12179,
            "min_price": 0.0325,
            "max_price": 69.42,
            "median_price": 0.59,
            "buyers": 5197,
            "sellers": 5777,
            "marketplaces": 1,
            "current_collection": "0x659a4bdaaacc62d2bd9cb18225d9c89b5b697a5a"
        },
        "trades_previous_week": null,
        "trades_current_month": {
            "volume": 8589.716710128467,
            "trades": 12179,
            "min_price": 0.0325,
            "max_price": 69.42,
            "median_price": 0.59,
            "buyers": 5197,
            "sellers": 5777,
            "marketplaces": 1,
            "current_collection": "0x659a4bdaaacc62d2bd9cb18225d9c89b5b697a5a"
        },
        "trades_previous_month": null,
        "name": "We Are All Going to Die",
        "symbol": "WAGDIE",
        "default_image": "https://media.niftyapi.xyz/0x659a4bdaaacc62d2bd9cb18225d9c89b5b697a5a/9",
        "slug": "we-are-all-going-to-die-4bdaaacc62d2bd9cb18225d9c89b5b697a5a",
        "decimals": "1",
        "first_block_seen": "14899270",
        "type": 721,
        "owner": "0xbf26fb48e19afe3dd99882c84016b8d16aae0636",
        "created_at": "2022-06-03T20:53:21.389Z",
        "nft_data_base_url": "ipfs://bafybeicpek2u6g7qtnlhrjw6sf54nw7nj3ae2ak5t6smegty2i42j3bvly/__TOKENID__",
        "nft_image_base_url": null,
        "metadata": null,
        "first_transfer": "2022-06-03T20:53:21.389Z"
    }],
    "query": "select * from \"nft_collection_stats\" left join \"collection\" on \"nft_collection_stats\".\"address\" = \"collection\".\"address\" order by (trades_current_day->>'volume')::numeric DESC  NULLS LAST limit 1",
    "page": 0,
    "perPage": 1
}
```

This endpoint retrieves all NFT trading data ordered orderBy parameter

### HTTP Request

`GET https://api.niftyapi.xyz/trades/collections?orderBy=volume_day`


### Query Parameters

| Parameter  | Default  | Description                     |
| ---------- | -------- | ------------------------------- |
| orderBy    |          | The field to sort by    |
| perPage    | 20       | Number of collections to return |
| page       | 1        | The page (for pagination)       |


| orderBy options (mandatory) |
| ------- |
| volume_hour |
| volume_day |
| volume_week |
| buyers_hour |
| buyers_day |
| buyers_week |
| sellers_hour |
| sellers_day |
| sellers_week |
| trades_hour |
| trades_day |
| trades_week |
| max_price_hour |
| max_price_day |
| max_price_week |
| min_price_hour |
| min_price_day |
| min_price_week |
| median_price_hour |
| median_price_day |
| median_price_week |