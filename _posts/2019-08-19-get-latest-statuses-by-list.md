---
apiurl: '/statuses/last'
title: 'Get the latest statuses by list of barcodes'
type: 'POST'

layout: default
---

This method allows the user to retrieve the latest statuses from the list of barcodes. You can send up to 100 barcodes in a request.
To receive the resonse in English, add **?lang=en** to the Url

### Request

* The headers must include a **valid authentication bearer**

```Authentication: Bearer 11111111-1111-1111-1111-111111111111```

Send a list of barcodes in the request body.

```
[  
   "0500100031143",
   "0500100031135"
]
```

### Response

Sends back a collection of the shipment statuses.

```Status: 200 OK```
```
[  
   {  
      "barcode":"0500100031143",
      "step":16,
      "date":"2017-07-29T20:24:00",
      "index":"65501",
      "name":"DKD ODESSA",
      "event":41000,
      "eventName":“Delivery",
      "country":"Ukraine",
      "eventReason":"personally",
      "eventReason_id":2,
      "mailType":1048576,
      "indexOrder":4
   },
   {  
      "barcode":"0500100031135",
      "step":16,
      "date":"2017-07-29T20:23:00",
      "index":"65501",
      "name":"DKD ODESSA",
      "event":41000,
      "eventName":“Delivery",
      "country":"Ukraine",
      "eventReason":"personally",
      "eventReason_id":2,
      "mailType":1048576,
      "indexOrder":4
   }
]

```

For errors responses, see the [response status codes documentation](#response-status-codes).