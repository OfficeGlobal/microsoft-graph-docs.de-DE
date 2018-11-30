---
title: Ressourcentyp emailAppUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 951d53f7491ff7f2b7721b14ed354d770cfd1730
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058756"
---
# <a name="emailappusageuserdetail-resource-type"></a>Ressourcentyp emailAppUsageUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ              |
| :---------------- | :---------------- |
| reportRefreshDate | Datum              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | Boolesch           |
| deletedDate       | Datum              |
| lastActivityDate  | Datum              |
| mailForMac        | Collection von Objekten des Typs „String“ |
| outlookForMac     | Collection von Objekten des Typs „String“ |
| outlookForWindows | Collection von Objekten des Typs „String“ |
| outlookForMobile  | Collection von Objekten des Typs „String“ |
| otherForMobile    | Collection von Objekten des Typs „String“ |
| outlookForWeb     | Collection von Objekten des Typs „String“ |
| pop3App           | Collection von Objekten des Typs „String“ |
| imap4App          | Collection von Objekten des Typs „String“ |
| smtpApp           | Collection von Objekten des Typs „String“ |
| reportPeriod      | String            |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "mailForMac": ["String"], 
  "outlookForMac": ["String"], 
  "outlookForWindows": ["String"], 
  "outlookForMobile": ["String"], 
  "otherForMobile": ["String"], 
  "outlookForWeb": ["String"], 
  "pop3App": ["String"], 
  "imap4App": ["String"], 
  "smtpApp": ["String"], 
  "reportPeriod": "String"
}
```
