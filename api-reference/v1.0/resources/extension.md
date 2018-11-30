---
title: extension-Ressourcentyp
description: Ein abstrakter Typ für die Unterstützung des offenen Typs openTypeExtension von OData v4.
ms.openlocfilehash: 1b3d735e0997ca128b539bff9a05c9c7c56799df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016255"
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
|id|String| Schreibgeschützt.|

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