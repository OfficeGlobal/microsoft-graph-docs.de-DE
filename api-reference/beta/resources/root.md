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
# <a name="root-resource-type"></a><span data-ttu-id="c9070-102">Root-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c9070-102">Root resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9070-103">Das **Root**-Facet gibt an, dass ein Objekt in der Hierarchie an der obersten Stelle steht.</span><span class="sxs-lookup"><span data-stu-id="c9070-103">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="c9070-104">Das Vorhandensein (Nicht-NULL) des Facetwerts gibt an, dass das Objekt der Stamm ist.</span><span class="sxs-lookup"><span data-stu-id="c9070-104">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="c9070-105">Ein Nullwert (oder ein fehlender Wert) bedeutet, dass das Objekt nicht der Stamm ist.</span><span class="sxs-lookup"><span data-stu-id="c9070-105">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="c9070-106">**Hinweis**: Dieses Facet ist heute zwar leer, in künftigen API-Überarbeitungen wird das Facet aber möglicherweise mit weiteren Eigenschaften gefüllt.</span><span class="sxs-lookup"><span data-stu-id="c9070-106">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9070-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c9070-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="c9070-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c9070-108">Properties</span></span>

<span data-ttu-id="c9070-109">Die **root**-Ressource hat keine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="c9070-109">The **Root** resource has no properties.</span></span>


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
