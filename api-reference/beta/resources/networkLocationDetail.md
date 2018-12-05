---
title: Ressourcentyp networkLocationDetail
description: Gibt den Speicherort im Netzwerk zugeordneten Details an. .
ms.openlocfilehash: 5dd1410318d380a1b943de6a7dbb0d739172cc76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062627"
---
# <a name="networklocationdetail-resource-type"></a>Ressourcentyp networkLocationDetail
Gibt den Speicherort im Netzwerk zugeordneten Details an. .



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|networkType|String|Stellt den Typ des Netzwerks. Mögliche Werte sind `intranet`, `extranet`, `namedNetwork`, und `trusted`.|
|Netzwerkname|String|Name des Netzwerks.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": "namedNetork",
  "networkName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->