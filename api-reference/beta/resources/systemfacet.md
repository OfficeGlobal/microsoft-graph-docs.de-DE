---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: SystemFacet
localization_priority: Normal
ms.openlocfilehash: afafb69e9d887d2cb8d9537dd7ef9d3a712f3333
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528550"
---
# <a name="system-facet"></a><span data-ttu-id="092f0-102">SystemFacet</span><span class="sxs-lookup"><span data-stu-id="092f0-102">System facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="092f0-103">Das **System**-Facette gibt an, dass das Objekt bei der eigenen Ausführung vom System verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="092f0-103">The **System** facet indicates that the object is managed by the system for its own operation.</span></span>
<span data-ttu-id="092f0-104">Die meisten Apps ignorieren Elemente mit System-Facette.</span><span class="sxs-lookup"><span data-stu-id="092f0-104">Most apps should ignore items that have a System facet.</span></span>

<span data-ttu-id="092f0-105">**Hinweis**: Dieses Facet ist heute zwar leer, in künftigen API-Überarbeitungen wird das Facet aber möglicherweise mit weiteren Eigenschaften gefüllt.</span><span class="sxs-lookup"><span data-stu-id="092f0-105">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="092f0-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="092f0-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.systemFacet", "@type.aka": "microsoft.graph.systemFacet" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="092f0-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="092f0-107">Properties</span></span>

<span data-ttu-id="092f0-108">Keine.</span><span class="sxs-lookup"><span data-stu-id="092f0-108">None.</span></span> <span data-ttu-id="092f0-109">Dieses Facet ist ein NULL- oder Nicht-NULL-Wert und enthält keine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="092f0-109">This facet is a null or not-null value and contains no properties.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/System",
  "suppressions": [
    "Error: /api-reference/beta/resources/systemfacet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
