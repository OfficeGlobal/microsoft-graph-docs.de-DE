---
title: Ressourcentyp emailAppUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1ebc99f25bf0b16343f48686496c1dbd7d329e65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977654"
---
# <a name="emailappusageuserdetail-resource-type"></a>Ressourcentyp emailAppUsageUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ              |
| :---------------- | :---------------- |
| reportRefreshDate | Datum              |
| userPrincipalName | Zeichenfolge            |
| displayName       | Zeichenfolge            |
| isDeleted         | Boolescher Wert           |
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
| reportPeriod      | Zeichenfolge            |

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
