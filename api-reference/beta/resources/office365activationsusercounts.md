---
title: Ressourcentyp office365ActivationsUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: f57393a538631664be8845fdaeda9f35d07c986f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849308"
---
# <a name="office365activationsusercounts-resource-type"></a>Ressourcentyp office365ActivationsUserCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft                 | Typ   | Beschreibung                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Datum   | Das aktuelle Datum des Inhalts.          |
| productType              | String | Der Produkttyp wie "Office 365 ProPlus", "Project-Client" oder "Visio Pro für Office 365". |
| zugewiesen                 | Int64  | Die Anzahl der Benutzer ist für die Produktlizenz zugewiesen worden. |
| aktiviert                | Int64  | Die Anzahl der Benutzer, die das Produkt aktiviert haben. |
| sharedComputerActivation | Int64  | Die Anzahl der Benutzer, die das Produkt auf einem freigegebenen Computer verwendet haben. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```
