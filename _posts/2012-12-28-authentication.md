---
path: '/login'
title: 'Authenticate'

layout: nil
---

The project helps You to integrate Your App with Ukrposta.

Authorization method

To access API use Bearer and Token.

Request format

curl -X {query_type} header 'Content-Type: application/json' --header 'Authorization: Bearer {bearer_Uuid}' 'https://www.ukrposhta.ua/{app-name}/{request}

where

{query_type} – request method: GET, POST, PUT, DELETE
Header: 'Authorization: Bearer {bearer_Uuid}' – parameter authorization bearer to get access
{app-name} – ecom/0.0.1
{request} – API endpoint.
For more information, please, visit our web-site

For errors responses, see the [response status codes documentation](#response-status-codes).
