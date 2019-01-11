---
title: Ressourcentyp mailboxUsageDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 25cb41e38138a677bfc6636b035003bb8fc5858c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818011"
---
# <a name="mailboxusagedetail-resource-type"></a>Ressourcentyp mailboxUsageDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                        | Typ    |
| :------------------------------ | :------ |
| reportRefreshDate               | Datum    |
| userPrincipalName               | String  |
| displayName                     | String  |
| isDeleted                       | Boolean |
| deletedDate                     | Datum    |
| createdDate                     | Datum    |
| lastActivityDate                | Datum    |
| itemCount                       | Int64   |
| storageUsedInBytes              | Int64   |
| issueWarningQuotaInBytes        | Int64   |
| prohibitSendQuotaInBytes        | Int64   |
| prohibitSendReceiveQuotaInBytes | Int64   |
| reportPeriod                    | String  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "createdDate": "Date", 
  "lastActivityDate": "Date", 
  "itemCount": 1024, 
  "storageUsedInBytes": 1024, 
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
