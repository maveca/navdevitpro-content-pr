---
title: Create salesQuotes | Microsoft Docs
description: Creates a sales quote object in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen

ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 03/19/2018
ms.author: solsen
---

# Create salesQuotes
Create a sales quote object in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request

```
POST /financials/companies({id})/salesQuotes
```

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required.    |
|Content-Type  |application/json    |

## Request body
In the request body, supply a JSON representation of a **salesQuotes** object.

## Response
If successful, this method returns ```201 Created``` response code and a **salesQuotes** object in the response body.

## Example

**Request**

Here is an example of a request.

```json
POST https://graph.microsoft.com/beta/financials/companies({id})/salesQuotes
Content-type: application/json

{
  "id": "id-value",
  "number": "1006",
  "documentDate": "2016-12-31",
  "customerNumber": "10000",
  "currencyCode": "GBP"
}
```
## See also
[Graph Reference](../api/dynamics_graph_reference.md)  
[Working with [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] in Microsoft Graph](../resources/dynamics_overview.md)  
[Error Codes](../dynamics_error_codes.md)  
[Sales Quote](../resources/dynamics_salesquote.md)  
[Get Sales Quote](../api/dynamics_salesquote_get.md)  
[Update Sales Quote](../api/dynamics_salesquote_update.md)  
[Delete Sales Quote](../api/dynamics_salesquote_delete.md)  