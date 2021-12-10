# Accounts

## Get All NFTs owned by an account

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

This endpoint retrieves all NFTs owned by an account.

### HTTP Request

`GET http://example.com/address/:address/`

### URL Parameters

| Parameter | Description                            |
| --------- | -------------------------------------- |
| Address   | The Address of the account to retrieve |
