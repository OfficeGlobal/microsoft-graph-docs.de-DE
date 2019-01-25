---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: 9b92a8234c493ae9b0f396db7010e7bf717d5959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514369"
---
# <a name="contenttypeorder-resource-type"></a>ContentTypeOrder-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **ContentTypeOrder**-Ressource gibt an, in welcher Reihenfolge der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **contentTypeOrder**-Ressource.
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname | Typ    | Beschreibung
|:--------------|:--------|:----------------------------------------------------
| **default**   | boolean | Gibt an, ob es sich  um den standardmäßigen Inhaltstyp handelt.
| **position**  | Int32   | Gibt die Position an, an welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": [
    "Error: /api-reference/beta/resources/contentTypeOrder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
