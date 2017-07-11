---
title: AgedAccountsPayable resource type | Microsoft Docs
description: A AgedAccountsPayable.
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

# Aged accounts payable resource type
Represents an agedAccountsPayable object in Dynamics 365 for Financials, which is showing the aging of a vendor account.

## Methods

| Method       | Return Type  |Description|
|:---------------|:--------|:----------|
|[GET agedAccountsPayable](../api/dynamics_get_agedaccountspayable.md)|AgedAccountsPayable|Get AgedAccountsPayable object|

## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|vendorId|GUID|The unique ID of vendor.|
|vendorNumber|string|Specifies vendor's number.|
|name|string|Specifies vendor's name.|
|currencyCode|string|Specifies the currency.|
|before|numeric|Specifies balance before first aging period.|
|period1|numeric|Specifies balance in the first aging period.|
|period2|numeric|Specifies balance in the second aging period.|
|period3|numeric|Specifies balance in the third aging period.|
|after|numeric|Specifies balance after third aging period.|
|balance|numeric|Specifies vendor's total balance.|
|periodStartDateFilter|date|Specifies period start date used to calculate aging periods.|
|periodLengthFilter|string|Specifies the length of the periods.|


## Relationships
None

## JSON representation

Here is a JSON representation of the resource.


```json
{
    "vendorId": "GUID",
    "vendorNumber": "string",
    "name": "string",
    "currencyCode": "string",
    "before": "decimal",
    "period1": "decimal",
    "period2": "decimal",
    "period3": "decimal",
    "after": "decimal",
    "balance": "decimal",
    "periodStartDateFilter": "date",
    "periodLengthFilter": "string
}

```
## See also
[Working with Dynamics 365 for Financials in Microsoft Graph](../resources/dynamics_overview.md) 