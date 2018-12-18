---
title: Ressourcentyp educationOrganization
description: 'Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.  '
author: mmast-msft
ms.openlocfilehash: 54f281de29033418b6acb2f9821c5ebd1eaf4db0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349889"
---
# <a name="educationorganization-resource-type"></a>Ressourcentyp educationOrganization

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.  

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|String| Beschreibung der Organisation.|
|displayName|String| Anzeigename der Organisation.|
|externalSource|string| Quelle, wo diese Organisation erstellt wurde. Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.|

## <a name="relationships"></a>Beziehungen
Keine.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->