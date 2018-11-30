---
title: Ressourcentyp referencedObject
description: Beschreibt einen Verweis auf ein anderes Objekt in der gleichen Verzeichnis Definition definiert.
ms.openlocfilehash: 63645048fd8ba6ad949da43baa261b2842ea4016
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065371"
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
            