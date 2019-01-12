---
title: Ressourcentyp mailboxUsageDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63b4b997a0ae559338fffd2acfabaa35dcc306e0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938734"
---
# <a name="mailboxusagedetail-resource-type"></a>Ressourcentyp mailboxUsageDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                        | Typ    |
| :------------------------------ | :------ |
| reportRefreshDate               | Datum    |
| userPrincipalName               | Zeichenfolge  |
| displayName                     | Zeichenfolge  |
| isDeleted                       | Boolescher Wert |
| deletedDate                     | Datum    |
| createdDate                     | Datum    |
| lastActivityDate                | Datum    |
| itemCount                       | Int64   |
| storageUsedInBytes              | Int64   |
| issueWarningQuotaInBytes        | Int64   |
| prohibitSendQuotaInBytes        | Int64   |
| prohibitSendReceiveQuotaInBytes | Int64   |
| reportPeriod                    | Zeichenfolge  |

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
