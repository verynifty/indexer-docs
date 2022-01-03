# Accounts

## Get All NFTs owned by an account

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "http://nft-data.vercel.app/address/:address/"
  );
```

> The above command returns JSON structured like this:

```json
[
  {
    "address":"0x224824908333b00be96fd4a52ada7f7597c22cba",
    "token_id":"443",
    "name":"Hidden Gamer Monkey",
    "description":"This Gamer Monkey is Unrevealed!",
    "external_url":null,
    "original_image":"https://lh3.googleusercontent.com/o-vEBAkFoTpxD_D3poIx7qOCm87fciKUNIxK3br3M0vzjhp1i6ESaNaImaVIR6GS6azo-hQN4eGdRDhK7tsBUFqw2UKjlIaia97GGw",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x224824908333b00be96fd4a52ada7f7597c22cba/443",
    "original_animation":null,
    "attributes":"",
    "metadata_type":4,
    "image_type":5,
    "owner":"0xdfd521971212e789b5ff05ef8d9f324fe290e238",
    "created_at":"2022-01-03T09:51:38.383Z",
    "updated_at":"2022-01-03T09:53:35.090Z",
    "latest_block_number":"13931782",
    "latest_log_index":"0",
    "search_weights":"'gamer':2A,5B 'hidden':1A 'monkey':3A,6B 'unrev':8B"
  },
  {
    "address":"0xad6dc35442d766f87f9296f17ba45e23518bc5f3",
    "token_id":"8947",
    "name":"Paladin Panda#8947",
    "description":"A PaladinPanda",
    "external_url":"https://www.paladinpandas.com/",
    "original_image":"https://product.ohdat.io/paladin_pandas/product/source/65.png",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0xad6dc35442d766f87f9296f17ba45e23518bc5f3/8947",
    "original_animation":"",
    "attributes":"\"Fur\"=>\"Leopard\", \"Class\"=>\"CyberBard\", \"Weapon\"=>\"Fan\", \"Bodygear\"=>\"Engineer\", \"Headgear\"=>\"Wizard\", \"Background\"=>\"Color3\", \"Expression\"=>\"Leopard Expression\"",
    "metadata_type":1,
    "image_type":1,
    "owner":"0xaa9772d31476e85fedd1099e40dd2ff5dee214ff",
    "created_at":"2021-12-29T08:15:36.905Z",
    "updated_at":"2021-12-29T08:15:38.493Z",
    "latest_block_number":"13899070",
    "latest_log_index":"0",
    "search_weights":"'8947':3A 'paladin':1A 'paladinpanda':5B 'panda':2A"
  },
  {
    "address":"0xf4cd7e65348deb24e30dedee639c4936ae38b763",
    "token_id":"4997",
    "name":"Galaktic Guy #4997",
    "description":"Welcome to the “Eternal Now” on the 5th dimension! In this mystical realm an army of alien spirits are joining forces to combat a vibrational war. The goal of “Galaktic Gang” is to bring balance back to the Universe, one planet at a time!",
    "external_url":null,
    "original_image":"ipfs://Qmdi1NXLrmeT9gzLPniQGQUDesRPifofxxsqDPFJfpyhL6/4997.png",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0xf4cd7e65348deb24e30dedee639c4936ae38b763/4997",
    "original_animation":null,
    "attributes":"\"Hat\"=>\"Locks Auburn\", \"Body\"=>\"Bling Starburst\", \"Ears\"=>\"Cans Jupiter\", \"Eyes\"=>\"Shades Inferno\", \"Halo\"=>\"Nothing\", \"Head\"=>\"Nugs Glacier\", \"Nose\"=>\"Stache Butterscotch\", \"Mouth\"=>\"Vocoder Jungle \", \"Cheeks\"=>\"Circuit Spectrum\", \"Background\"=>\"Peeling Bodies\"",
    "metadata_type":5,
    "image_type":4,
    "owner":"0x1846f080015ab53c7a16ab463b5e6aad61b0ab5d",
    "created_at":"2021-12-31T10:29:38.588Z",
    "updated_at":"2021-12-31T10:29:42.222Z",
    "latest_block_number":"13912608",
    "latest_log_index":"0","search_weights":"'4997':3A '5th':11B 'alien':20B 'armi':18B 'back':39B 'balanc':38B 'bring':37B 'combat':26B 'dimens':12B 'etern':7B 'forc':24B 'galakt':1A,33B 'gang':34B 'goal':31B 'guy':2A 'join':23B 'mystic':15B 'one':43B 'planet':44B 'realm':16B 'spirit':21B 'time':47B 'univers':42B 'vibrat':28B 'war':29B 'welcom':4B"
  }
]
```

This endpoint retrieves all NFTs owned by an account.

### HTTP Request

`GET http://nft-data.vercel.app/address/:address/`

### URL Parameters

| Parameter | Description                            |
| --------- | -------------------------------------- |
| Address   | The Address of the account to retrieve |
