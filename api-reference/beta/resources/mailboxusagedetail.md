---
title: Ressourcentyp mailboxUsageDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: af49fac7c6286c7e9f9ce1e6d7ffdede225b4072
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059795"
---
# <a name="mailboxusagedetail-resource-type"></a>Ressourcentyp mailboxUsageDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                        | Typ    |
| :------------------------------ | :------ |
| reportRefreshDate               | Datum    |
| userPrincipalName               | String  |
| displayName                     | String  |
| isDeleted                       | Boolesch |
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
