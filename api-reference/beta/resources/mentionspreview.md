---
title: Ressourcentyp mentionsPreview
description: Stellt Informationen zu Objekten in einer Ressourceninstanz einer Erwähnung dar.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 55eb69d9ef9f6c3686026f6d46a9c78cc4df167b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518765"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="50984-103">Ressourcentyp mentionsPreview</span><span class="sxs-lookup"><span data-stu-id="50984-103">mentionsPreview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50984-104">Stellt Informationen zu Objekten in einer Ressourceninstanz einer [erwähnen](../resources/mention.md) .</span><span class="sxs-lookup"><span data-stu-id="50984-104">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="50984-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="50984-105">Properties</span></span>
| <span data-ttu-id="50984-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50984-106">Property</span></span>     | <span data-ttu-id="50984-107">Typ</span><span class="sxs-lookup"><span data-stu-id="50984-107">Type</span></span>   |<span data-ttu-id="50984-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50984-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="50984-109">isMentioned</span><span class="sxs-lookup"><span data-stu-id="50984-109">isMentioned</span></span> | <span data-ttu-id="50984-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="50984-110">Boolean</span></span> | <span data-ttu-id="50984-111">True, wenn die angemeldeten Benutzers in der Instanz des übergeordneten Ressource genannt wird.</span><span class="sxs-lookup"><span data-stu-id="50984-111">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="50984-112">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="50984-112">Read-only.</span></span> <span data-ttu-id="50984-113">Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="50984-113">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="50984-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="50984-114">JSON representation</span></span>

<span data-ttu-id="50984-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="50984-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mentionspreview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
