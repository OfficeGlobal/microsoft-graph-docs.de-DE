---
title: Ressourcentyp office365ActivationsUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0d5ed2af02f429f5fd4d6e92b408d2e8e420f4d0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574544"
---
# <a name="office365activationsusercounts-resource-type"></a>Ressourcentyp office365ActivationsUserCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft                 | Typ   | Beschreibung                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Date   | Das aktuelle Datum des Inhalts.          |
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
