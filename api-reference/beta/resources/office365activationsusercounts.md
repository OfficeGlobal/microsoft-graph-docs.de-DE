---
title: Ressourcentyp office365ActivationsUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3dc497e516f95f1e05167703f2b9f8aea6363a64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917720"
---
# <a name="office365activationsusercounts-resource-type"></a>Ressourcentyp office365ActivationsUserCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft                 | Typ   | Beschreibung                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Datum   | Das aktuelle Datum des Inhalts.          |
| productType              | Zeichenfolge | Der Produkttyp wie "Office 365 ProPlus", "Project-Client" oder "Visio Pro für Office 365". |
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
