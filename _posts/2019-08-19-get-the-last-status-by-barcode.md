---
apiurl: '/statuses/last?barcode=barcode'
title: 'Get the last status by barcode'
type: 'GET'

layout: default
---

This method allows the user to retrieve the last shipment status by barcode.

### Request

* **`:barcode`** is a brcode of the shipment.
* The headers must include a **valid authentication bearer**.
* **The body is empty**.

```Authentication: Bearer 11111111-1111-1111-1111-111111111111```

### Response

Sends back a collection of the shipment statuses.

```Status: 200 OK```
```
[     
     {  
      "barcode":"0500100031143",
      "step":3,
      "date":"2017-07-27T16:33:00",
      "index":"03505",
      "name":"DKD KYIV",
      "event":10100,
      "eventName":“Acceptance",
      "country":"Ukraine",
      "eventReason":null,
      "eventReason_id":1,
      "mailType":1048576,
      "indexOrder":1
    }
]
```

For errors responses, see the [response status codes documentation](#response-status-codes).