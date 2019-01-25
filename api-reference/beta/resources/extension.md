---
title: extension-Ressourcentyp
description: Ein abstrakter Typ für die Unterstützung des offenen Typs openTypeExtension von OData v4.
localization_priority: Normal
ms.openlocfilehash: b261ceeff4639b8a602edbb411b34ab19d46ea8e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512745"
---
# <a name="extension-resource-type"></a>extension-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein abstrakter Typ für die Unterstützung des offenen Typs [openTypeExtension](opentypeextension.md) von OData v4.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/extension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
