---
title: licenseUnitsDetail-Ressourcentyp
description: Die **prepaidUnits**-Eigenschaft der subscribedSku-Entität ist vom Typ **licenseUnitsDetail**.
ms.openlocfilehash: 5f3d62c39248739746923195945efbc3322d5686
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058206"
---
# <a name="licenseunitsdetail-resource-type"></a>licenseUnitsDetail-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **prepaidUnits**-Eigenschaft der [subscribedSku](subscribedsku.md)-Entität ist vom Typ **licenseUnitsDetail**.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:-------------|:-----|:----------|
|aktiviert|Int32| Die Anzahl der Einheiten, die aktiviert werden. |
|suspended|Int32| Die Anzahl der Einheiten, die angehalten werden. |
|warning|Int32| Die Anzahl der Einheiten, für die eine Warnung vorliegt. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
