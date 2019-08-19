---
apiurl: '/statuses?barcode=barcode'
title: 'Get all statuses by barcode'
type: 'GET'

layout: default
---

This method allows the user to retrieve all shipment statuses by barcode.

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
    },
    {  
      "barcode":"0500100031143",
      "step":2,
      "date":"2017-07-27T16:51:57",
      "index":"03505",
      "name":"DKD KYIV",
      "event":20700,
      "eventName":“Arrival”,
      "country":"Ukraine",
      "eventReason":null,
      "eventReason_id":1,
      "mailType":1048576,
      "indexOrder":1
    },
    {  
      "barcode":"0500100031143",
      "step":4,
      "date":"2017-07-27T16:58:18",
      "index":"03505",
      "name":"DKD KYIV",
      "event":20800,
      "eventName":“Shipment",
      "country":"Ukraine",
      "eventReason":null,
      "eventReason_id":1,
      "mailType":1048576,
      "indexOrder":1
    },
    {  
      "barcode":"0500100031143",
      "step":5,
      "date":"2017-07-27T18:26:30",
      "index":"03909",
      "name":"DOPP KYIV",
      "event":20700,
      "eventName":“Arrival”,
      "country":"Ukraine",
      "eventReason":null,
      "eventReason_id":1,
      "mailType":1048576,
      "indexOrder":2
    },
    {  
      "barcode":"0500100031143",
      "step":8,
      "date":"2017-07-27T22:52:23",
      "index":"03909",
      "name":"DOPP KYIV",
      "event":20800,
      "eventName":“Shipment",
      "country":"Ukraine",
      "eventReason":null,
      "eventReason_id":1,
      "mailType":1048576,
      "indexOrder":2
    },
    {  
      "barcode":"0500100031143",
      "step":9,
      "date":"2017-07-28T08:50:12",
      "index":"65399",
      "name":“TSEHOP ODESSA”,
      "event":20700,
      "eventName":“Arrival”,
      "country":"Ukraine",
      "eventReason":null,
      "eventReason_id":1,
      "mailType":1048576,
      "indexOrder":3
    },
    {  
      "barcode":"0500100031143",
      "step":12,
      "date":"2017-07-28T09:49:28",
      "index":"65399",
      "name":“TSEHOP ODESSA”,
      "event":20800,
      "eventName":“Shipment",
      "country":"Ukraine",
      "eventReason":null,
      "eventReason_id":1,
      "mailType":1048576,
      "indexOrder":3
    },
    {  
      "barcode":"0500100031143",
      "step":14,
      "date":"2017-07-28T09:49:45",
      "index":"65501",
      "name":"DKD ODESSA",
      "event":21500,
      "eventName":“Sending to branch office”,
      "country":"Ukraine",
      "eventReason":null,
      "eventReason_id":1,
      "mailType":1048576,
      "indexOrder":4
    },
    {  
      "barcode":"0500100031143",
      "step":15,
      "date":"2017-07-28T18:41:00",
      "index":"65501",
      "name":"DKD ODESSA",
      "event":21700,
      "eventName":“Arrival to the branch office”,
      "country":"Ukraine",
      "eventReason":null,
      "eventReason_id":1,
      "mailType":1048576,
      "indexOrder":4
    },
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
    }
]
```

For errors responses, see the [response status codes documentation](#response-status-codes).