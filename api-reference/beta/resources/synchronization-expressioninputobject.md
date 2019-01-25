---
title: Ressourcentyp expressionInputObject
description: 'Stellt ein Objekt als Eingabe Testdaten verwendet werden bei der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion ausführt Ausdruck in Bezug auf.'
localization_priority: Normal
ms.openlocfilehash: 3e631102505408b955404c4badb33b98f314236f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510778"
---
# <a name="expressioninputobject-resource-type"></a>Ressourcentyp expressionInputObject

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt ein Objekt als Eingabe Testdaten verwendet werden bei der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion ausführt Ausdruck in Bezug auf.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|definition|[Sind](synchronization-objectdefinition.md)|Definition des Test-Objekts.|
|properties|[StringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) -Auflistung|Eigenschaftswerte des Test-Objekts.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-expressioninputobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
