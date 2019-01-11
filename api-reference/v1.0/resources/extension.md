---
title: extension-Ressourcentyp
description: Ein abstrakter Typ für die Unterstützung des offenen Typs openTypeExtension von OData v4.
localization_priority: Normal
ms.openlocfilehash: 2633c8a28c1be1a670a80834ce869b5156fc1de9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834671"
---
# <a name="extension-resource-type"></a>extension-Ressourcentyp

Ein abstrakter Typ für die Unterstützung des offenen Typs [openTypeExtension](opentypeextension.md) von OData v4.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "abstract": "true",
  "baseType": "microsoft.graph.entity",
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|Zeichenfolge| Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="methods"></a>Methoden

Informationen zu tatsächlich unterstützten Methoden finden Sie in den Methoden des abgeleiteten Typs [openTypeExtension](opentypeextension.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
