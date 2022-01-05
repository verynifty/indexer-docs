# NFTs

## Get All NFTs in a collection

```javascript
const axios = require("axios");

let { data: nfts } = await axios(
  "https://nft-data.vercel.app/collection/nfts/0xc3f733ca98e0dad0386979eb96fb1722a1a05e69"
);
```

> The above command returns JSON structured like this:

```json
[
  {
    "address":"0xe3435edbf54b5126e817363900234adfee5b3cee",
    "token_id":"9994",
    "name":"Voxie #9994",
    "description":"Voxies are cute, lovable and collectible voxel buddies, that live and play on the Ethereum blockchain. There are only 10,000 Voxies in existence and no two Voxies are identical. Lots of random properties and fun traits make each Voxie cute, unique and sometimes rare!",
    "external_url":"https://voxies.io",
    "original_image":"https://voxies-data-final-2.s3.us-east-2.amazonaws.com/9994.gif",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0xe3435edbf54b5126e817363900234adfee5b3cee/9994",
    "original_animation":"https://voxies-data-final-2.s3.us-east-2.amazonaws.com/9994.mp4",
    "attributes":"\"Item\"=>\"Dragon Bow\", \"Luck\"=>\"7\", \"Race\"=>\"Zombie\", \"Armor\"=>\"7\", \"Class\"=>\"Monster\", \"Emote\"=>\"Zombie Walk\", \"Ground\"=>\"Grass\", \"Rarity\"=>\"Common\", \"Outline\"=>\"Cartoon\", \"Movement\"=>\"4\", \"Strength\"=>\"8\", \"Dexterity\"=>\"7\", \"Background\"=>\"Space\", \"Top Costume\"=>\"Mage\", \"Intelligence\"=>\"2\", \"Bottom Costume\"=>\"Druid\"",
    "metadata_type":1,
    "image_type":1,
    "owner":"0x3c38bf9e4189117ba75816e9e01c9d627b5810c3",
    "created_at":"2022-01-03T11:27:18.389Z",
    "updated_at":"2022-01-03T11:27:26.544Z",
    "latest_block_number":"13932182",
    "latest_log_index":"0",
    "search_weights":"'000':23B '10':22B '9994':2A 'blockchain':18B 'buddi':10B 'collect':8B 'cute':5B,43B 'ethereum':17B 'exist':26B 'fun':38B 'ident':32B 'live':12B 'lot':33B 'lovabl':6B 'make':40B 'play':14B 'properti':36B 'random':35B 'rare':47B 'sometim':46B 'trait':39B 'two':29B 'uniqu':44B 'voxel':9B 'voxi':1A,3B,24B,30B,42B"
  },
  {
    "address":"0x97e41d5ce9c8cb1f83947ef82a86e345aed673f3",
    "token_id":"264",
    "name":"Ninja #264",
    "description":null,
    "external_url":null,
    "original_image":"https://theninjahideout.mypinata.cloud/ipfs/QmevApYR33NXqeLkCezocNat8RsnYBAzG5DpHPDwG5FZhz/264.png",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x97e41d5ce9c8cb1f83947ef82a86e345aed673f3/264",
    "original_animation":null,
    "attributes":"\"Body\"=>\"Light\", \"Eyes\"=>\"Green\", \"Mouth\"=>\"Mouth Scar\", \"Sword\"=>\"Wrapped Handle\", \"Agility\"=>\"7\", \"Clothing\"=>\"Green Dress Shirt\", \"Headband\"=>\"Sun\", \"Ornament\"=>\"Small Leaf\", \"Strength\"=>\"6\", \"Hairstyle\"=>\"Messy (Blue)\", \"Background\"=>\"Beach\", \"Intelligence\"=>\"10\"",
    "metadata_type":1,
    "image_type":1,
    "owner":"0xb79252d4fb3d61a0590f9c156612926496f897a4",
    "created_at":"2022-01-03T11:10:04.173Z",
    "updated_at":"2022-01-03T11:10:09.747Z",
    "latest_block_number":"13932104",
    "latest_log_index":"0",
    "search_weights":"'264':2A 'ninja':1A"
  },
  {
    "address":"0x1f0f72e6dc2ea6fde3a32a1b3fd47a26a3293dc9",
    "token_id":"3524",
    "name":"Lamb Duh #3524",
    "description":"A collection of 8,500 digital lambs wandering the grasslands of the Ethereum blockchain!",
    "external_url":"https://www.lambduhs.com",
    "original_image":"https://gateway.pinata.cloud/ipfs/QmVJFHpc6XQGxytGUPsgbLanPoDFpc6D8acvFeP3HG5aZZ",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x1f0f72e6dc2ea6fde3a32a1b3fd47a26a3293dc9/3524",
    "original_animation":null,
    "attributes":"\"Body\"=>\"Flannel\", \"Face\"=>\"Tongue\", \"Head\"=>\"Military Helmet\", \"Tier\"=>\"Delta\", \"Wool\"=>\"Green\"",
    "metadata_type":1,
    "image_type":4,
    "owner":"0xbfceb6a652b5ab0b3d19f0142efe71dcf6d062c3",
    "created_at":"2022-01-02T05:30:01.515Z",
    "updated_at":"2022-01-02T05:30:04.604Z",
    "latest_block_number":"13924146",
    "latest_log_index":"0",
    "search_weights":"'3524':3A '500':8B '8':7B 'blockchain':17B 'collect':5B 'digit':9B 'duh':2A 'ethereum':16B 'grassland':13B 'lamb':1A,10B 'wander':11B"
  },
  {
    "address":"0xbbe23e96c48030dc5d4906e73c4876c254100d33",
    "token_id":"504",
    "name":"RebelBot #00504",
    "description":"#00504 is a 1st generation Rebelbot. Factory code: DRCO",
    "external_url":null,
    "original_image":"ipfs://QmcVzAaGoWVGwz4oCHjRoUwyy6vzd8RSmkrNAFHZBwN6rE",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0xbbe23e96c48030dc5d4906e73c4876c254100d33/504",
    "original_animation":null,
    "attributes":"\"Hat\"=>\"Pony tail hair\", \"Eyes\"=>\"Angry\", \"Skin\"=>\"Bronze metal\", \"Mouth\"=>\"Cigarette\", \"Clothes\"=>\"Rebel Bots red t-shirt\", \"Background\"=>\"Grey\"",
    "metadata_type":1,
    "image_type":4,
    "owner":"0xbd584ce590b7dcdbb93b11e095d9e1d5880b44d9","created_at":"2022-01-03T06:20:24.453Z",
    "updated_at":"2022-01-03T11:35:00.828Z",
    "latest_block_number":"13932213",
    "latest_log_index":"314",
    "search_weights":"'00504':2A,3B '1st':6B 'code':10B 'drco':11B 'factori':9B 'generat':7B 'rebelbot':1A,8B"
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
  "http://nft-data.vercel.app/nft/0xc3f733ca98e0dad0386979eb96fb1722a1a05e69/7120"
);
```

> The above command returns JSON structured like this:

```json
[
  {
    "address":"0x93a796b1e846567fe3577af7b7bb89f71680173a",
    "token_id":"4563",
    "name":null,
    "description":"We are warrior ChainFaces. Here to watch over you forever, unless we get eaten by lions.",
    "external_url":null,
    "original_image":"https://storage.opensea.io/files/d603f58c181aea1faab1daa1a324ae1b.svg",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x93a796b1e846567fe3577af7b7bb89f71680173a/4563",
    "original_animation":null,
    "attributes":"",
    "metadata_type":4,
    "image_type":5,
    "owner":"0x9435ce0dc1f0565036bd0f9e3f4334c01f8b9762",
    "created_at":"2022-01-02T01:53:09.424Z",
    "updated_at":"2022-01-02T02:22:46.447Z",
    "latest_block_number":"13923303",
    "latest_log_index":"200",
    "search_weights":"'chainfac':4B 'eaten':14B 'forev':10B 'get':13B 'lion':16B 'unless':11B 'warrior':3B 'watch':7B"
  },
  {
    "address":"0xc1a1e381389cb927f1d57511e144b644ef0c6385",
    "token_id":"41",
    "name":"LOSTBOY 41",
    "description":"[Animation (.mp4)](https://lostboy.mypinata.cloud/ipfs/QmSxLpp3cjQf8eYtaJgQyX6ddWd8UuDVh2WWkms9kbzJPG)\n\n[Music (.mp3)](https://lostboy.mypinata.cloud/ipfs/QmXinzRqvG8cYUr5wFP5oVYCJcaph1BkxPKzh7wUJnFRQb})\n\n[Image (.png)](https://lostboy.mypinata.cloud/ipfs/QmfYm4ich2d9M5tQJWpLTBSo9387TTrQT2SddcDhmGwNRH)\n\n",
    "external_url":null,
    "original_image":"https://lostboy.mypinata.cloud/ipfs/QmfYm4ich2d9M5tQJWpLTBSo9387TTrQT2SddcDhmGwNRH",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0xc1a1e381389cb927f1d57511e144b644ef0c6385/41",
    "original_animation":"https://lostboy.mypinata.cloud/ipfs/QmSxLpp3cjQf8eYtaJgQyX6ddWd8UuDVh2WWkms9kbzJPG",
    "attributes":"\"Mouth\"=>\"Covid Mask\", \"Music\"=>\"Better Days\", \"Shoes\"=>\"Tye Dye Crocks\", \"Head/Eye\"=>\" Headband\", \"Accessory\"=>\"No Accessory\", \"Background\"=>\"Rainbow Aura\", \"Upper Wear\"=>\"Meow Hoodie\", \"Bottom Wear\"=>\"Donut Shorts\"",
    "metadata_type":1,
    "image_type":1,
    "owner":"0xc1e637c9fcac6dfebc4df52f2610a2c6b12b4d02",
    "created_at":"2022-01-02T16:58:45.200Z",
    "updated_at":"2022-01-02T16:58:54.434Z",
    "latest_block_number":"13927255",
    "latest_log_index":"0",
    "search_weights":"'/ipfs/qmfym4ich2d9m5tqjwpltbso9387ttrqt2sddcdhmgwnrh)':17B '/ipfs/qmsxlpp3cjqf8eytajgqyx6ddwd8uudvh2wwkms9kbzjpg)':7B '/ipfs/qmxinzrqvg8cyur5wfp5ovycjcaph1bkxpkzh7wujnfrqb':12B '41':2A 'anim':3B 'imag':13B 'lostboy':1A 'lostboy.mypinata.cloud':6B,11B,16B 'lostboy.mypinata.cloud/ipfs/qmfym4ich2d9m5tqjwpltbso9387ttrqt2sddcdhmgwnrh)':15B 'lostboy.mypinata.cloud/ipfs/qmsxlpp3cjqf8eytajgqyx6ddwd8uudvh2wwkms9kbzjpg)':5B 'lostboy.mypinata.cloud/ipfs/qmxinzrqvg8cyur5wfp5ovycjcaph1bkxpkzh7wujnfrqb':10B 'mp3':9B 'mp4':4B 'music':8B 'png':14B"
  },
  {
    "address":"0x1e38e9ad28a526512af9b8689c50d91443b6c3db",
    "token_id":"4763",
    "name":"Pukenza #4763",
    "description":"Pukenza (also known as Rainbow over the Flow Field), inspired by Tyler Hobb's Fidenza, uses similar concepts combined with Doodles' color palette to create aesthetically soothing generative art. Funded by Doodlebank and created by L3xc from Degen Art Club.",
    "external_url":null,
    "original_image":"ipfs://QmVEzQPgfuatRPeAzeZh8MGRv5MnecSg2vdQXfZPFRK18R",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x1e38e9ad28a526512af9b8689c50d91443b6c3db/4763",
    "original_animation":null,
    "attributes":"\"seed\"=>\"0xe480fe1c90f4de0afa4baa84686b6f95e144edd60abdc2a1e3c320e908ee509d\", \"gaussy\"=>\"no\", \"spiral\"=>\"no\", \"density\"=>\"medium\", \"flowiness\"=>\"high\", \"generator\"=>\"Doodle #4763\", \"background\"=>\"dark\", \"max thiccness\"=>\"normal\", \"min thiccness\"=>\"thicc af\", \"continous lines\"=>\"yes\", \"brightness filter\"=>\"low\", \"saturation filter\"=>\"high\"",
    "metadata_type":1,
    "image_type":4,
    "owner":"0xdddf58fab219f9bf28228d6b5fcf9e97970811ff",
    "created_at":"2022-01-02T06:16:29.070Z",
    "updated_at":"2022-01-02T06:16:33.480Z",
    "latest_block_number":"13924360",
    "latest_log_index":"0",
    "search_weights":"'4763':2A 'aesthet':28B 'also':4B 'art':31B,41B 'club':42B 'color':24B 'combin':21B 'concept':20B 'creat':27B,36B 'degen':40B 'doodl':23B 'doodlebank':34B 'fidenza':17B 'field':11B 'flow':10B 'fund':32B 'generat':30B 'hobb':15B 'inspir':12B 'known':5B 'l3xc':38B 'palett':25B 'pukenza':1A,3B 'rainbow':7B 'similar':19B 'sooth':29B 'tyler':14B 'use':18B"

  },
  {
    "address": "0x280f2599693159a96e367b621670840fcff06ee2",
    "token_id": "2245",
    "name": "Cosmic Mice",
    "description": "Races of mice fight together in this degen friendly PvP experiment",
    "external_url": null,
    "original_image": "https://lh3.googleusercontent.com/y1Yg9XgllhAIN3yYT27PZzeOEcOXOCwp7Q6icMdBlGtSaWsEXLkOCqmATjMRLIQY8MgqDAGEoce3YrXHVzdHAkmdBuK9SpIvolvh_4c",
    "image": "https://d3nt5b5e09uon7.cloudfront.net/0x280f2599693159a96e367b621670840fcff06ee2/2245",
    "original_animation": null,
    "attributes": "",
    "metadata_type": 4,
    "image_type": 5,
    "owner": "0x5af1c6c005ce3b0238304d022ef5fa5b240fcc55",
    "created_at": "2022-01-02T01:20:06.302Z",
    "updated_at": "2022-01-02T11:24:27.458Z",
    "latest_block_number": "13925689",
    "latest_log_index": "398",
    "search_weights": "'cosmic':1A 'degen':10B 'experi':13B 'fight':6B 'friend':11B 'mice':2A,5B 'pvp':12B 'race':3B 'togeth':7B"
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
  "http://nft-data.vercel.app/transfers/0xc3f733ca98e0dad0386979eb96fb1722a1a05e69/7120"
);
```

> The above command returns JSON structured like this:

```json
[
  {

    "collection":"0xfcb1315c4273954f74cb16d5b663dbf479eec62e",
    "block_number":"13902932",
    "transaction_hash":"0x3df4326d26cd6d24d60c4ac150e5cf8f17bdd555de5e35087fc64769b842a161","transaction_index":"125",
    "tx_to":"0x7be8076f4ea4a4ad08075c2508e481d6c946d12b",
    "tx_from":"0x3bad10ac78d7d653e10a6747151a91b08c866f75",
    "log_index":"263",
    "transfer_index":"0",
    "timestamp":"2021-12-29T22:26:38.000Z",
    "to":"0x3bad10ac78d7d653e10a6747151a91b08c866f75",
    "from":"0x3c6b176c1e44d5423fd946f876fa9a1793df4c3e",
    "amount":"1",
    "token_id":"1809",
    "gas_price":"98406694153",
    "created_at":"2021-12-29T22:27:40.028Z",
    "address":"0xfcb1315c4273954f74cb16d5b663dbf479eec62e",
    "name":"01809",
    "description":"Capsule House is a collection of 10,000 unique gachapon NFTs - a digital version of the collectible toys popular in Japan. With over 100 species, 60 variants, and endless combinations of traits, each Capsule NFT contains a verifiably rare and unique gachapon artwork. Holding a Capsule grants you to future drops from the team, as well as an all access pass to the expansion of the CAPSULEVerse. Visit https://capsulehouse.io for more details.",
    "external_url":"https://capsulehouse.io",
    "original_image":"https://tunes.mypinata.cloud/ipfs/QmWUcSn7pciRwsEnPd4whUzvbmbYRm4dVGaPn16X3D6dHF/01809.png",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0xfcb1315c4273954f74cb16d5b663dbf479eec62e/1809",
    "original_animation":null,
    "attributes":"\"Mouth\"=>\"Bandaid\", \"Chroma\"=>\"Hidden Ruby\", \"Purity\"=>\"Augmented\", \"Eyewear\"=>\"Square Glasses\", \"Species\"=>\"Humans\", \"Variant\"=>\"Pirate\", \"Decorative\"=>\"Fast Food\", \"Generation\"=>\"Psi\"",
    "metadata_type":1,
    "image_type":1,
    "owner":"0x3bad10ac78d7d653e10a6747151a91b08c866f75",
    "updated_at":"2021-12-29T22:27:49.836Z",
    "latest_block_number":"13902932",
    "latest_log_index":"0",
    "search_weights":"'000':9B '01809':1A '10':8B '100':25B '60':27B 'access':61B 'artwork':44B 'capsul':2B,35B,47B 'capsulehouse.io':70B 'capsulevers':68B 'collect':6B,18B 'combin':31B 'contain':37B 'detail':73B 'digit':14B 'drop':52B 'endless':30B 'expans':65B 'futur':51B 'gachapon':11B,43B 'grant':48B 'hold':45B 'hous':3B 'japan':22B 'nft':36B 'nfts':12B 'pass':62B 'popular':20B 'rare':40B 'speci':26B 'team':55B 'toy':19B 'trait':33B 'uniqu':10B,42B 'variant':28B 'verifi':39B 'version':15B 'visit':69B 'well':57B"
  },
  {
    "collection":"0x3fe1a4c1481c8351e91b64d5c398b159de07cbc5",
    "block_number":"13914820",
    "transaction_hash":"0xc241efb22e60d94cb91db5fa56b88342180c7db60adf4496279e1aaa23243838",
    "transaction_index":"196",
    "tx_to":"0x7be8076f4ea4a4ad08075c2508e481d6c946d12b",
    "tx_from":"0x3786efe23d0f22342d19131676c8542c384e853d",
    "log_index":"364",
    "transfer_index":"0",
    "timestamp":"2021-12-31T18:55:43.000Z",
    "to":"0x3786efe23d0f22342d19131676c8542c384e853d",
    "from":"0x9c73959f4462c5ad98182c141385cc95820310d4",
    "amount":"1",
    "token_id":"1803",
    "gas_price":"88720462873",
    "created_at":"2021-12-31T18:58:30.348Z",
    "address":"0x3fe1a4c1481c8351e91b64d5c398b159de07cbc5",
    "name":"SupDuck 1803",
    "description":null,
    "external_url":"https://www.supducks.com/",
    "original_image":"https://ipfs.io/ipfs/QmS3SXQHuwgVzGtzj2oTcgDntvPoDBMYXHK2VAotmJwDZo",
    "image":"https://d3nt5b5e09uon7.cloudfront.net/0x3fe1a4c1481c8351e91b64d5c398b159de07cbc5/1803",
    "original_animation":null,
    "attributes":"\"Hat\"=>\"Hair\", \"Eyes\"=>\"Super Happy\", \"Skin\"=>\"White Pebble\", \"Mouth\"=>\"WhaWha\", \"Clothes\"=>\"Itchy Ass Sweater\", \"Background\"=>\"Green\"",
    "metadata_type":5,
    "image_type":1,
    "owner":"0x3786efe23d0f22342d19131676c8542c384e853d",
    "updated_at":"2021-12-31T18:58:34.145Z",
    "latest_block_number":"13914820",
    "latest_log_index":"0",
    "search_weights":"'1803':2A 'supduck':1A"

  },
  {
    "collection": "0x280f2599693159a96e367b621670840fcff06ee2",
    "block_number": "13925857",
    "transaction_hash": "0xfdceb7f8dd26df7c115b0fc5bcdb7a63cb55a32eb39b116e6813f16f2daee26f",
    "transaction_index": "186",
    "tx_to": "0x0a267cf51ef038fc00e71801f5a524aec06e4f07",
    "tx_from": "0xf0a5043111c2a35fbd1acfb588c382e781ad6aef",
    "log_index": "207",
    "transfer_index": "0",
    "timestamp": "2022-01-02T12:02:50.000Z",
    "to": "0xf0a5043111c2a35fbd1acfb588c382e781ad6aef",
    "from": "0x72df07d6cb06d55b4e38f0b3761e0406e3fb38f6",
    "amount": "1",
    "token_id": "973",
    "gas_price": "51839405234",
    "created_at": "2022-01-02T01:13:32.938Z",
    "address": "0x280f2599693159a96e367b621670840fcff06ee2",
    "name": "Cosmic Mice",
    "description": "Races of mice fight together in this degen friendly PvP experiment",
    "external_url": null,
    "original_image": "ipfs://QmUkYRYSK4NhdF7CcrUA1F73ESDJcCiVARNHWh2QS4vLsE/hidden.gif",
    "image": "https://d3nt5b5e09uon7.cloudfront.net/0x280f2599693159a96e367b621670840fcff06ee2/973",
    "original_animation": null,
    "attributes": null,
    "metadata_type": 5,
    "image_type": 4,
    "owner": "0xf0a5043111c2a35fbd1acfb588c382e781ad6aef",
    "updated_at": "2022-01-02T12:03:56.459Z",
    "latest_block_number": "13925857",
    "latest_log_index": "207",
    "search_weights": "'cosmic':1A 'degen':10B 'experi':13B 'fight':6B 'friend':11B 'mice':2A,5B 'pvp':12B 'race':3B 'togeth':7B"
  },
  {
    "collection": "0x280f2599693159a96e367b621670840fcff06ee2",
    "block_number": "13923004",
    "transaction_hash": "0xf7c9e1b7bc683ef08d6c63ef3bfec43373f6cb9f5798bccb6f73ae45f59c4718",
    "transaction_index": "161",
    "tx_to": "0x280f2599693159a96e367b621670840fcff06ee2",
    "tx_from": "0x72df07d6cb06d55b4e38f0b3761e0406e3fb38f6",
    "log_index": "268",
    "transfer_index": "0",
    "timestamp": "2022-01-02T01:11:21.000Z",
    "to": "0x72df07d6cb06d55b4e38f0b3761e0406e3fb38f6",
    "from": "0x0000000000000000000000000000000000000000",
    "amount": "1",
    "token_id": "973",
    "gas_price": "68811070431",
    "created_at": "2022-01-02T01:13:32.938Z",
    "address": "0x280f2599693159a96e367b621670840fcff06ee2",
    "name": "Cosmic Mice",
    "description": "Races of mice fight together in this degen friendly PvP experiment",
    "external_url": null,
    "original_image": "ipfs://QmUkYRYSK4NhdF7CcrUA1F73ESDJcCiVARNHWh2QS4vLsE/hidden.gif",
    "image": "https://d3nt5b5e09uon7.cloudfront.net/0x280f2599693159a96e367b621670840fcff06ee2/973",
    "original_animation": null,
    "attributes": null,
    "metadata_type": 5,
    "image_type": 4,
    "owner": "0xf0a5043111c2a35fbd1acfb588c382e781ad6aef",
    "updated_at": "2022-01-02T12:03:56.459Z",
    "latest_block_number": "13925857",
    "latest_log_index": "207",
    "search_weights": "'cosmic':1A 'degen':10B 'experi':13B 'fight':6B 'friend':11B 'mice':2A,5B 'pvp':12B 'race':3B 'togeth':7B"
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
