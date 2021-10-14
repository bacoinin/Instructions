Alrighty, so here are some instructions for the seller to complete. It shouldn't be too complicated, but its always good to ensure that its the right buyer that you're resending messages to... which is why its a little more drawn out than what it should be).

NB!! I've also made the assumption here that the seller is selling from the particl-market identity. If they've created and are using an alternative identity the last step below is going to need to change.

Steps:

1. Open the Market Console Window: Market module > Market Settings > Open Marketplace Console button

2. Type in the following command: `orderitem history X`

3. The output should be a list of the messages relating to the orderitem. Looks something similar to the following:
```
[
    {
      "id": 3,
      "type": "MPA_LISTING_ADD_03",
      "status": "PROCESSED",
      "direction": "INCOMING",
      "target": null,
      "msgid": "000000006148544ce0dd84c8918ba519336a2026146bed1f72e9ca3a",
      "version": "0300",
      "read": 1,
      "paid": 1,
      "payloadsize": 1216,
      "received": 1632130674000,
      "sent": 1632130124000,
      "expiration": 1632216524000,
      "daysretention": 1,
      "from": "PdEiGvq9h9t3VZP5Z7qMTFx9MStBpQ8r9D",
      "to": "Pa2fZ7Jgka4NWG3UfPFDYuGqmMrzAa7BP6",
      "text": "{\"version\":\"3.0.0\",\"action\":{\"type\":\"MPA_LISTING_ADD_03\",\"generated\":1632130029809,\"item\":{\"information\":{\"title\":\"sample product\", ...",
      "processedCount": 1,
      "processedAt": 1632130674508,
      "updatedAt": 1632130674786,
      "createdAt": 1632130674478
    },
    {
      "id": 5,
      "type": "MPA_BID_03",
      "status": "PROCESSED",
      "direction": "INCOMING",
      "target": null,
      "msgid": "00000000614856e3325506920f06b3a66c99528b753abf0a4b8ecc8c",
      "version": "0201",
      "read": 1,
      "paid": 0,
      "payloadsize": 1552,
      "received": 1632130797000,
      "sent": 1632130787000,
      "expiration": 1632735587000,
      "daysretention": 7,
      "from": "Ps9wEMba289izGUTgCsRZ5rSMDqT5PXveg",
      "to": "PuKJWubrtfTpxTUNFmEMgTvjrKJAmwrDzx",
      "text": "{\"version\":\"3.0.0\",\"action\":{\"type\":\"MPA_BID_03\",\"hash\":\"dd8b3dcfb2756118ae647f4627d183abf74be1d77667cbeb4079f6eda798f337\", ...",
      "processedCount": 1,
      "processedAt": 1632130797483,
      "updatedAt": 1632130797579,
      "createdAt": 1632130797452
    },
    {
      "id": 6,
      "type": "MPA_ACCEPT_03",
      "status": "SENT",
      "direction": "OUTGOING",
      "target": null,
      "msgid": "0000000061485ba8ba7684fa66d66dc706da9019ddc69ee5db4e0a0f",
      "version": "0201",
      "read": 0,
      "paid": 0,
      "payloadsize": 1712,
      "received": 1632132008000,
      "sent": 1632132008000,
      "expiration": 1632736808000,
      "daysretention": 7,
      "from": "PuKJWubrtfTpxTUNFmEMgTvjrKJAmwrDzx",
      "to": "Ps9wEMba289izGUTgCsRZ5rSMDqT5PXveg",
      "text": "{\"version\":\"3.0.0\",\"action\":{\"type\":\"MPA_ACCEPT_03\",\"hash\":\"\",\"generated\":1632132008057,\"bid\":\"dd8b3dcfb2756118ae647f4627d183abf74be1d77667cbeb4079f6eda798f337 ..."
      "processedCount": 0,
      "processedAt": 0,
      "updatedAt": 1632132008587,
      "createdAt": 1632132008587
    },
    {
      "id": 7,
      "type": "MPA_LOCK_03",
      "status": "PROCESSED",
      "direction": "INCOMING",
      "target": null,
      "msgid": "0000000061485bbbf2c5393d9b36d28355d14e5f0ee6daad78b4197b",
      "version": "0201",
      "read": 1,
      "paid": 0,
      "payloadsize": 1216,
      "received": 1632132037000,
      "sent": 1632132027000,
      "expiration": 1632736827000,
      "daysretention": 7,
      "from": "Ps9wEMba289izGUTgCsRZ5rSMDqT5PXveg",
      "to": "PuKJWubrtfTpxTUNFmEMgTvjrKJAmwrDzx",
      "text": " ... ",
      "processedCount": 1,
      "processedAt": 1632132037502,
      "updatedAt": 1632132037629,
      "createdAt": 1632132037486
    },
    {
      "id": 8,
      "type": "MPA_COMPLETE",
      "status": "SENT",
      "direction": "OUTGOING",
      "target": null,
      "msgid": "0000000061485d412eed43e5be79ae08e1bb2f2685ca815d4284083a",
      "version": "0201",
      "read": 0,
      "paid": 0,
      "payloadsize": 432,
      "received": 1632132417000,
      "sent": 1632132417000,
      "expiration": 1632737217000,
      "daysretention": 7,
      "from": "PuKJWubrtfTpxTUNFmEMgTvjrKJAmwrDzx",
      "to": "Ps9wEMba289izGUTgCsRZ5rSMDqT5PXveg",
      "text": " ... ",
      "processedCount": 0,
      "processedAt": 0,
      "updatedAt": 1632132417905,
      "createdAt": 1632132417905
    },
    {
      "id": 9,
      "type": "MPA_SHIP",
      "status": "SENT",
      "direction": "OUTGOING",
      "target": null,
      "msgid": "0000000061485d7bcf5bd6ac952eef1161254f76d32454a62928921a",
      "version": "0201",
      "read": 0,
      "paid": 0,
      "payloadsize": 384,
      "received": 1632132475000,
      "sent": 1632132475000,
      "expiration": 1632737275000,
      "daysretention": 7,
      "from": "PuKJWubrtfTpxTUNFmEMgTvjrKJAmwrDzx",
      "to": "Ps9wEMba289izGUTgCsRZ5rSMDqT5PXveg",
      "text": " ... ",
      "processedCount": 0,
      "processedAt": 0,
      "updatedAt": 1632132475828,
      "createdAt": 1632132475828
    }
  ]
```
4. In the item in the list with the "type" value of "MPA_BID_03", the "text field should contain some information that shows the buyer's shipping address, for example: "SHIPPING_BID\",\"firstName\":\"abcdefg\",\"lastName\":\"hijklmn\",\"addressLine1\":\"111111\" ... . The seller can confirm that the details are the correct ones, so they know they have the correct buyer.

Additionally, if the same buyer has bought something else as well, an added check is that there should be no object in the list that has the type of "MPA_RELEASE"

5. Once its confirmed that the correct OrderItem is being looked at, find the statuses that have the "type" fields

 - "MPA_COMPLETE"
 - "MPA_SHIP"

6. In each of those statuses, there is the "msgid" field: copy the value from each status out. For example, using the previous status, the values we're looking at would be 0000000061485d412eed43e5be79ae08e1bb2f2685ca815d4284083a and 0000000061485d7bcf5bd6ac952eef1161254f76d32454a62928921a

7. Now to resend each of those messages: starting with the msgid value from the MPA_COMPLETE status, input the following into the market console window for each of the 2 values (wait a couple seconds before sending the 2nd message): smsg resend <msgid> 1 replacing <msgid> with the actual msgid value. For example: smsg resend 0000000061485d412eed43e5be79ae08e1bb2f2685ca815d4284083a 1 followed by smsg resend 0000000061485d7bcf5bd6ac952eef1161254f76d32454a62928921a 1 after a few seconds.
  
