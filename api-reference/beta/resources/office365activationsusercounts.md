---
title: Ressourcentyp office365ActivationsUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 90d9d2d8616f166eb9d8b87967898daa0468db54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064738"
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
