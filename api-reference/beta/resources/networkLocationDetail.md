---
title: Ressourcentyp networkLocationDetail
description: Gibt den Speicherort im Netzwerk zugeordneten Details an. .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643762"
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
