---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Stamm
localization_priority: Normal
ms.openlocfilehash: dda2de3e92128a9813f923d9acfef0eec94680e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510302"
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
