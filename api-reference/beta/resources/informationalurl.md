---
title: Ressourcentyp informationalUrl
description: Grundlegende Profilinformationen der Anwendung.
localization_priority: Normal
ms.openlocfilehash: 5085c144045631c530cbb66f5e1f27186a63b380
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513648"
---
# <a name="informationalurl-resource-type"></a>Ressourcentyp informationalUrl

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Grundlegende Profilinformationen der Anwendung.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|"Marketing"|String| Link zu marketing Anwendungsseite. Beispiel: https://www.contoso.com/app/marketing |
|Datenschutz|String| Link zu Datenschutzrichtlinie für die Anwendung. Beispiel: https://www.contoso.com/app/privacy |
|Support|String| Link zu der Anwendung Supportseite. Beispiel: https://www.contoso.com/app/support |
|termsOfService|String| Link zu der Anwendung Begriffe der Service-Anweisung. Beispiel: https://www.contoso.com/app/termsofservice |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/informationalurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
