# Collections

## Get All Collections

```javascript
const axios = require("axios");

let { data: collections } = await axios("api");
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

This endpoint retrieves all collections.

### HTTP Request

`GET http://example.com/collections`

### Query Parameters

| Parameter | Default | Description                     |
| --------- | ------- | ------------------------------- |
| perPage   | 10      | Number of collections to return |
| page      | 0       | The page (for pagination)       |

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Get a Specific colletction

```javascript
const axios = require("axios");

let { data: collection } = await axios("api");
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific collection.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET http://example.com/collection/:address/<ID>`

### URL Parameters

| Parameter | Description                               |
| --------- | ----------------------------------------- |
| Address   | The Address of the collection to retrieve |
