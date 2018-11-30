---
title: Ressourcentyp parseExpressionResponse
description: 'Stellt die Antwort von der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion.'
ms.openlocfilehash: 625df0ca16135eaa35c5b679c79dea582c4012e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065190"
---
# <a name="parseexpressionresponse-resource-type"></a>Ressourcentyp parseExpressionResponse

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Antwort von der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|error|OData.Error|Fehlerdetails, wenn die Auswertung von Ausdrücken ein Fehler aufgetreten.|
|evaluationResult|Collection von Objekten des Typs „String“|Eine Auflistung von Werten, die mit der Auswertung des Ausdrucks.|
|evaluationSucceeded|Boolesch|`true`Wenn die Auswertung erfolgreich war.|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|Ein [AttributeMappingSource](synchronization-attributemappingsource.md) -Objekt, das den analysierten Ausdruck darstellt.|
|parsingSucceeded|Boolesch|`true`Wenn der Ausdruck erfolgreich analysiert wurde.|

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
<!-- {
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->