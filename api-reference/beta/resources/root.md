---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Stamm
localization_priority: Normal
ms.openlocfilehash: 8c320a34d22af5fc73a1c5d8c96dce14e176946f
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482371"
---
# <a name="root-resource-type"></a>Root-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Das **Root**-Facet gibt an, dass ein Objekt in der Hierarchie an der obersten Stelle steht.
Das Vorhandensein (Nicht-NULL) des Facetwerts gibt an, dass das Objekt der Stamm ist.
Ein Nullwert (oder ein fehlender Wert) bedeutet, dass das Objekt nicht der Stamm ist.

**Hinweis**: Dieses Facet ist heute zwar leer, in künftigen API-Überarbeitungen wird das Facet aber möglicherweise mit weiteren Eigenschaften gefüllt.

## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a>Eigenschaften

Die **root**-Ressource hat keine Eigenschaften.


<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root",
  "suppressions": [
    "Error: /api-reference/beta/resources/root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
