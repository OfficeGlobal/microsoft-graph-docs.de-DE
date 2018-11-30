---
title: Ressourcentyp userActivationCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 022b73310a54877889efebabbb6e8fc4ab71fb65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061139"
---
# <a name="useractivationcounts-resource-type"></a>Ressourcentyp userActivationCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   | Beschreibung                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | String | Produkttyp, beispielsweise "Office 365 ProPlus", "Project-Client" oder "Visio Pro für Office 365". |
| lastActivatedDate | Datum   | Das Datum der neuesten Aktivierung.       |
| Windows           | Int64  | Die Anzahl der Aktivierung auf Windows. Dieser Wert schließt alle Aktivierung auf einem beliebigen Windows-Computer. |
| mac               | Int64  | Die Anzahl der Aktivierung auf Mac OS.          |
| windows10Mobile   | Int64  | Die Aktivierung zählen auf 10 für Windows mobile. |
| IOS               | Int64  | Die Anzahl der Aktivierung auf iOS.             |
| Android (engl.)           | Int64  | Die Anzahl der Aktivierung auf einer Android-Gerät.  |
| activatedOnSharedComputer   | Boolesch | True, wenn der Benutzer das Produkt auf einem freigegebenen Computer vor verwendet. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userActivationCounts"
} -->

```json
{
  "productType": "String", 
  "lastActivatedDate": "Date", 
  "windows": 1024, 
  "mac": 1024, 
  "windows10Mobile": 1024, 
  "ios": 1024, 
  "android": 1024,
  "activatedOnSharedComputer": true 
}
```
