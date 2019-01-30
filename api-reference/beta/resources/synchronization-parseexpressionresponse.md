---
title: Ressourcentyp parseExpressionResponse
description: 'Stellt die Antwort von der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion.'
localization_priority: Normal
ms.openlocfilehash: f8ea708468e1e580693b2bd0e6f0e7f3494996f0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641057"
---
# <a name="parseexpressionresponse-resource-type"></a>Ressourcentyp parseExpressionResponse

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt die Antwort von der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|error|OData.Error|Fehlerdetails, wenn die Auswertung von Ausdrücken ein Fehler aufgetreten.|
|evaluationResult|String-Sammlung|Eine Auflistung von Werten, die mit der Auswertung des Ausdrucks.|
|evaluationSucceeded|Boolean|`true`Wenn die Auswertung erfolgreich war.|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|Ein [AttributeMappingSource](synchronization-attributemappingsource.md) -Objekt, das den analysierten Ausdruck darstellt.|
|parsingSucceeded|Boolean|`true`Wenn der Ausdruck erfolgreich analysiert wurde.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parseExpressionResponse"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.publicError"},
  "evaluationResult": ["String"],
  "evaluationSucceeded": true,
  "parsedExpression": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "parsingSucceeded": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-parseexpressionresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
