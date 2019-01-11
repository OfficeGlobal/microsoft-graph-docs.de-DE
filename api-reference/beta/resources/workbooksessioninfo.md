---
title: workbookSessionInfo-Ressourcentyp
description: Enthält Informationen zu Arbeitsmappensitzungen.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 25812d48626c7dc5e468915f7308941a4f74b38e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860963"
---
# <a name="workbooksessioninfo-resource-type"></a>workbookSessionInfo-Ressourcentyp

Enthält Informationen zu Arbeitsmappensitzungen.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ  | Beschreibung                               |
|:---------|:------|:------------------------------------------|
| id  | string | Die ID der Arbeitsmappensitzung. |
| persistChanges | string |  `true` für eine beständige Sitzung `false` für eine nicht-beständige Sitzung (Ansichtsmodus) |

