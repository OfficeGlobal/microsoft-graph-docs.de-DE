---
title: workbookSessionInfo-Ressourcentyp
description: Enthält Informationen zu Arbeitsmappensitzungen.
author: lumine2008
ms.openlocfilehash: 1e097cad70a6058aab28ad85d7cf6b3c3b52ac75
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305985"
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
| persistChanges | Boolean |  `true` für eine beständige Sitzung `false` für eine nicht-beständige Sitzung (Ansichtsmodus) |

