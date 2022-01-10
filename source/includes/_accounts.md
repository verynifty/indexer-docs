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
  }
]
```

This endpoint retrieves all NFTs owned by an account.

### HTTP Request

`GET https://api.niftyapi.xyz/address/:address/`

### URL Parameters

| Parameter | Description                            |
| --------- | -------------------------------------- |
| Address   | The Address of the account to retrieve |
