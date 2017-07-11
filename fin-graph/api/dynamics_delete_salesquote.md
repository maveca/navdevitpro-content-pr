---
title: DELETE sales quote method | Microsoft Docs
description: Deletes a sales quote.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen

ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/11/2017
ms.author: solsen
---

# Delete sales quote
Delete a sales quote from Dynamics 365 for Financials.


## HTTP request
```
DELETE /financials/companies/{id}/salesQuotes/{id}
```

## Request headers
|Header|Value|
|------|-----|
|Authorization  |Bearer. Required. |
|If-Match      |Required. When this request header is included and the eTag provided does not match the current tag on the salesQuotes, the salesQuotes will not be updated. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.

## Example

**Request**

Here is an example of the request.

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/salesQuotes/{id}
```

**Response** 

Here is an example of the response. 

```json
HTTP/1.1 204 No Content
```

## See also
[Working with Dynamics 365 for Financials in Microsoft Graph](../resources/dynamics_overview.md) 