---
title: Ressourcentyp networkLocationDetail
description: Gibt den Speicherort im Netzwerk zugeordneten Details an. .
localization_priority: Normal
ms.openlocfilehash: 62bdb23c63beb89b85386e6bea67face097cf1ae
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570939"
---
# <a name="networklocationdetail-resource-type"></a>Ressourcentyp networkLocationDetail
Gibt den Speicherort im Netzwerk zugeordneten Details an. .



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|networkType| Enum-Zeichenfolge |Stellt den Typ des Netzwerks. Mögliche Werte sind `intranet`, `extranet`, `namedNetwork`, und `trusted`.|
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
  "networkTypes": " intranet | extranet | namedNetwork | trusted ",
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
