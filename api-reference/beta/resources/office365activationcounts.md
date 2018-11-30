---
title: Ressourcentyp office365ActivationCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: e53a979ac627735ef63a24e1823d83f4c9fe9f7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064760"
---
# <a name="office365activationcounts-resource-type"></a>Ressourcentyp office365ActivationCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   | Beschreibung                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Datum   | Das aktuelle Datum des Inhalts.          |
| productType       | String | Produkttyp, beispielsweise "Office 365 ProPlus", "Project-Client" oder "Visio Pro für Office 365". |
| Windows           | Int64  | Die Anzahl der Aktivierung auf Windows. Dieser Wert schließt alle Aktivierung auf einem beliebigen Windows-Computer. |
| mac               | Int64  | Die Anzahl der Aktivierung auf Mac OS.          |
| Android (engl.)           | Int64  | Die Anzahl der Aktivierung auf einer Android-Gerät.  |
| IOS               | Int64  | Die Anzahl der Aktivierung auf iOS.             |
| windows10Mobile   | Int64  | Die Aktivierung zählen auf 10 für Windows mobile. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```
