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
# <a name="root-resource-type"></a><span data-ttu-id="3c580-102">Root-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3c580-102">Root resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c580-103">Das **Root**-Facet gibt an, dass ein Objekt in der Hierarchie an der obersten Stelle steht.</span><span class="sxs-lookup"><span data-stu-id="3c580-103">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="3c580-104">Das Vorhandensein (Nicht-NULL) des Facetwerts gibt an, dass das Objekt der Stamm ist.</span><span class="sxs-lookup"><span data-stu-id="3c580-104">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="3c580-105">Ein Nullwert (oder ein fehlender Wert) bedeutet, dass das Objekt nicht der Stamm ist.</span><span class="sxs-lookup"><span data-stu-id="3c580-105">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="3c580-106">**Hinweis**: Dieses Facet ist heute zwar leer, in künftigen API-Überarbeitungen wird das Facet aber möglicherweise mit weiteren Eigenschaften gefüllt.</span><span class="sxs-lookup"><span data-stu-id="3c580-106">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c580-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3c580-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="3c580-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3c580-108">Properties</span></span>

<span data-ttu-id="3c580-109">Die **root**-Ressource hat keine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="3c580-109">The **Root** resource has no properties.</span></span>


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
