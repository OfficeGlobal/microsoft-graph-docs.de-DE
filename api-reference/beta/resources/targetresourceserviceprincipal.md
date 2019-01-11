---
title: Ressourcentyp targetResourceServicePrincipal
description: Gibt die ServicePrincipalId für die Ressource, die die Audit-Aktivität betroffen. Die Ressource TargetResource abgeleitet.
localization_priority: Normal
ms.openlocfilehash: 37bd63851ca9169afb669c710ef4cb2c150ea615
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839599"
---
# <a name="targetresourceserviceprincipal-resource-type"></a>Ressourcentyp targetResourceServicePrincipal
Gibt die ServicePrincipalId für die Ressource, die die Audit-Aktivität betroffen. Die Ressource [TargetResource](targetresource.md) abgeleitet.



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|appId|Zeichenfolge|Gibt die eindeutige Id der Anwendung an. Verweist auf die App-Id für eine angegebene app.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceServicePrincipal"
}-->

```json
{
  "appId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
