---
title: Ressourcentyp referencedObject
description: Beschreibt einen Verweis auf ein anderes Objekt in der gleichen Verzeichnis Definition definiert.
localization_priority: Normal
ms.openlocfilehash: 5a2aa2dcc358c856c18ea2ce9871ec634194ce54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821035"
---
# <a name="referencedobject-resource-type"></a>Ressourcentyp referencedObject

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Beschreibt einen Verweis auf ein anderes Objekt in der gleichen [Verzeichnis Definition](synchronization-directorydefinition.md)definiert.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                   | Typ                      | Beschreibung    |
|:---------------------------|:--------------------------|:---------------|
|referencedObjectName        |String                     |Name des Objekts verwiesen wird. Muss eines der Objekte in der [Definition des Verzeichnisses](synchronization-directorydefinition.md)übereinstimmen.|
|referencedProperty          |String                     |**Derzeit nicht unterstützt**. Der Name der Eigenschaft in das Objekt verwiesen wird, der, das Wert für die als Referenz verwendet wird.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referencedObject"
}-->

```json
{
  "referencedObjectName": "String",
  "referencedProperty": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
            
