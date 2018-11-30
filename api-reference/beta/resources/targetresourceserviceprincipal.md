---
title: Ressourcentyp targetResourceServicePrincipal
description: Gibt die ServicePrincipalId für die Ressource, die die Audit-Aktivität betroffen. Die Ressource TargetResource abgeleitet.
ms.openlocfilehash: 6d6e19997f4bfead771fc0230207df62dde6c6cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064064"
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