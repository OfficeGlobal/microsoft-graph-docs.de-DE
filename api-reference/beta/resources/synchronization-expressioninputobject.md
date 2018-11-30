---
title: Ressourcentyp expressionInputObject
description: 'Stellt ein Objekt als Eingabe Testdaten verwendet werden bei der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion ausführt Ausdruck in Bezug auf.'
ms.openlocfilehash: 06b7344f7e6418db0557f2b12dfa7e964b9d5ab7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064998"
---
# <a name="expressioninputobject-resource-type"></a>Ressourcentyp expressionInputObject

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
<!-- {
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->