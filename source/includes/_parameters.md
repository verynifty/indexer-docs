# Parameters

## Search query

The search ('s') query parameter is used to filter return NFTs by name or id. Any name or id that contains the query parameter string will be returned.

e.g. s=25 will return any NFT with id and name that contains '25'

```javascript
const axios = require("axios");

let collection = "0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d"
let searchString = "5555"
let url = `https://api.niftyapi.xyz/collection/nfts/${collection}?s=${searchString}`
let { data: nfts } = await axios(url);
```

> Response

```json
{
   "nfts": [{
      "address": "0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d",
      "token_id": "5555",
      "name": null,
      "description": null,
      "external_url": "https://gateway.ipfs.io/ipfs/QmeSjSinHpPnmXmspMjwiXyN6zS4E9zccariGR3jxcaWtq/5555",
      "image": "https://media.niftyapi.xyz/0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d/5555",
      "attributes": "\"Fur\"=>\"Dark Brown\", \"Hat\"=>\"Army Hat\", \"Eyes\"=>\"Bored\", \"Mouth\"=>\"Bored Unshaven Cigarette\", \"Clothes\"=>\"Black Suit\", \"Earring\"=>\"Silver Hoop\", \"Background\"=>\"Yellow\"",
      "image_type": 4,
      "owner": "0xeab974fae1582aa8707586b836c7b6313c47992f",
      "created_at": "2022-01-24T08:08:58.779Z",
      "updated_at": "2022-05-22T23:22:48.112Z",
      "latest_block_number": "14826194"
   }]
}
```

## Attributes

The 'attributes' query parameter is used to filter returned NFTs by query

A URI encoded json object value should be passed for attribute query parameter

> e.g Lets say we want to get only NFTs with 'Background' value of 'Orange'

```json
{"Background":["Orange"]}
```

> encode json using URI encoding into

```
%7B%22Background%22%3A%5B%22Orange%22%5D%7D
```

> Complete HTTP example

```
GET https://api.niftyapi.xyz/address/0x900647fd2d4af5b3bb21d98b3aa6d3cc49b35ced?collection=0x6ff683ea4ba14aa2a0fa3ca927b7886dba827b65&attributes=%7B%22Background%22%3A%5B%22Orange%22%5D%7D`
```

```javascript
const axios = require("axios");

let userAddress = "0x900647fd2d4af5b3bb21d98b3aa6d3cc49b35ced"
let collection = "0x6ff683ea4ba14aa2a0fa3ca927b7886dba827b65"
let attributes = encodeURIComponent(JSON.stringify({"Background":["Orange"]}))
let url = `https://api.niftyapi.xyz/address/${userAddress}?collection=${collection}&attributes=${attributes}`
let { data: nfts } = await axios(url);

```

> Should return below result

```json
[
   {
      "address":"0x6ff683ea4ba14aa2a0fa3ca927b7886dba827b65",
      "token_id":"2875",
      "name":"pepe mfer #2875",
      "description":"A total of 7000 Pepes mfers created. This project is in the public domain for the community to do as they please. 10% of the initial sale will be sent to the mfer treasury.  Like Sartoshi said:  \"Discord\" - no, we don’t; mfers built one for mfers \"Roadmap\" - no, mfers are paving their own roads \"Paid promos\" - no, mfers move organically \"Utility\" - mfers are the utility mfer",
      "external_url":"https://gateway.ipfs.io/ipfs/bafybeia24ckqc3qi5zg57j2wsclgqbfkmziixy5grlgctjljmhpco7ejde/2875.json",
      "image":"https://media.niftyapi.xyz/0x6ff683ea4ba14aa2a0fa3ca927b7886dba827b65/2875",
      "attributes":"\"Body\"=>\"Brown\", \"Eyes\"=>\"Purple Shades\", \"Head\"=>\"Mohawk Yellow\", \"Mouth\"=>\"Smile\", \"Shirt\"=>\"Collared Shirt Black\", \"Background\"=>\"Orange\", \"Headphones\"=>\"Black Headphones\"",
      "image_type":4,
      "owner":"0x900647fd2d4af5b3bb21d98b3aa6d3cc49b35ced",
      "created_at":"2022-03-10T16:36:49.236Z",
      "updated_at":"2022-05-29T01:35:24.671Z",
      "latest_block_number":"14863680",
      "collection_name":"Pepe mfers",
      "collection_symbol":"pm"
   }
]
```
