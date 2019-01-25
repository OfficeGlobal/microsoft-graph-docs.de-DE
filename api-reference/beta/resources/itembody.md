---
title: itemBody-Ressourcentyp
description: Stellt Eigenschaften des Textkörpers eines Elements dar, z. B. eine Nachricht, ein Ereignis oder ein Gruppenbeitrag.
localization_priority: Normal
ms.openlocfilehash: f316beda82f292e62d5063f45363e08eeeff7111
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526144"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="f13dc-103">itemBody-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f13dc-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f13dc-104">Stellt Eigenschaften des Textkörpers eines Elements dar, z. B. eine Nachricht, ein Ereignis oder ein Gruppenbeitrag.</span><span class="sxs-lookup"><span data-stu-id="f13dc-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="f13dc-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f13dc-105">Properties</span></span>
| <span data-ttu-id="f13dc-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f13dc-106">Property</span></span>     | <span data-ttu-id="f13dc-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f13dc-107">Type</span></span>   |<span data-ttu-id="f13dc-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f13dc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f13dc-109">Inhalt</span><span class="sxs-lookup"><span data-stu-id="f13dc-109">content</span></span>|<span data-ttu-id="f13dc-110">String</span><span class="sxs-lookup"><span data-stu-id="f13dc-110">String</span></span>|<span data-ttu-id="f13dc-111">Der Inhalt des Elements.</span><span class="sxs-lookup"><span data-stu-id="f13dc-111">The content of the item.</span></span>|
|<span data-ttu-id="f13dc-112">contentType</span><span class="sxs-lookup"><span data-stu-id="f13dc-112">contentType</span></span>|<span data-ttu-id="f13dc-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f13dc-113">String</span></span>|<span data-ttu-id="f13dc-p101">Der Typ des Inhalts. Mögliche Werte sind `Text` und `HTML`.</span><span class="sxs-lookup"><span data-stu-id="f13dc-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f13dc-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f13dc-116">JSON representation</span></span>

<span data-ttu-id="f13dc-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f13dc-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/itembody.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
