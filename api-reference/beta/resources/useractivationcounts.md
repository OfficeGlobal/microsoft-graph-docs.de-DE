---
title: Ressourcentyp userActivationCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: dkershaw10
ms.openlocfilehash: 396f6182d000df6d701e8c0cbad3dd02a258c4c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322918"
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
