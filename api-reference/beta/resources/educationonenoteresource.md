---
title: Ressourcentyp educationOneNoteResource
description: 'Eine Unterklasse der EducationResource. Dies ist den Speicherort der OneNote-Seite.  '
author: mmast-msft
ms.openlocfilehash: dc6fc6a71da12a27cb589e072371814e4bc33cc1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359864"
---
# <a name="educationonenoteresource-resource-type"></a>Ressourcentyp educationOneNoteResource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine Unterklasse der [EducationResource](educationresource.md). Dies ist den Speicherort der OneNote-Seite.  

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|pageUrl|String|Die Microsoft Graph-URL zu der Seite in OneNote.|
|sectionName|String|Im Abschnittsname, die Verteilung in kopiert werden sollte oder in kopiert wurden.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
