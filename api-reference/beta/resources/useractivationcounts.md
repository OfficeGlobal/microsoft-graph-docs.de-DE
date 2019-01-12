---
title: Ressourcentyp userActivationCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 535355d6be3f6b617d7eb293890aa05a517cfc3b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980349"
---
# <a name="useractivationcounts-resource-type"></a>Ressourcentyp userActivationCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   | Beschreibung                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | Zeichenfolge | Produkttyp, beispielsweise "Office 365 ProPlus", "Project-Client" oder "Visio Pro für Office 365". |
| lastActivatedDate | Datum   | Das Datum der neuesten Aktivierung.       |
| Windows           | Int64  | Die Anzahl der Aktivierung auf Windows. Dieser Wert schließt alle Aktivierung auf einem beliebigen Windows-Computer. |
| mac               | Int64  | Die Anzahl der Aktivierung auf Mac OS.          |
| windows10Mobile   | Int64  | Die Aktivierung zählen auf 10 für Windows mobile. |
| IOS               | Int64  | Die Anzahl der Aktivierung auf iOS.             |
| Android (engl.)           | Int64  | Die Anzahl der Aktivierung auf einer Android-Gerät.  |
| activatedOnSharedComputer   | Boolescher Wert | True, wenn der Benutzer das Produkt auf einem freigegebenen Computer vor verwendet. |

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
