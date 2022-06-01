# Parameters

## Search query

search query

## Attributes

The 'attributes' query parameter to used to filter returned NFTs by query

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
GET https://api.niftyapi.xyz/address/0x900647fd2d4af5b3bb21d98b3aa6d3cc49b35ced?page=1&perPage=30&collection=0x6ff683ea4ba14aa2a0fa3ca927b7886dba827b65&attributes=%7B%22Background%22%3A%5B%22Orange%22%5D%7D`
```

```javascript
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
