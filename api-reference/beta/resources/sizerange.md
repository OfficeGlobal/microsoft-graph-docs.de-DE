---
title: sizeRange-Ressourcentyp
description: Gibt die maximale und minimale Größe (in Kilobyte) an, die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.
localization_priority: Normal
ms.openlocfilehash: ecf4a4349e7ee54b9f21fa27879834b45dc87491
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522399"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="2230f-103">sizeRange-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2230f-103">sizeRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2230f-104">Gibt die maximale und minimale Größe (in Kilobyte) an, die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.</span><span class="sxs-lookup"><span data-stu-id="2230f-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="2230f-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2230f-105">Properties</span></span>
| <span data-ttu-id="2230f-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2230f-106">Property</span></span>     | <span data-ttu-id="2230f-107">Typ</span><span class="sxs-lookup"><span data-stu-id="2230f-107">Type</span></span>   |<span data-ttu-id="2230f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2230f-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2230f-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="2230f-109">maximumSize</span></span> | <span data-ttu-id="2230f-110">Int32</span><span class="sxs-lookup"><span data-stu-id="2230f-110">Int32</span></span> | <span data-ttu-id="2230f-111">Die maximale Größe (in Kilobyte), die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.</span><span class="sxs-lookup"><span data-stu-id="2230f-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="2230f-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="2230f-112">minimumSize</span></span> | <span data-ttu-id="2230f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="2230f-113">Int32</span></span> | <span data-ttu-id="2230f-114">Die minimale Größe (in Kilobyte), die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.</span><span class="sxs-lookup"><span data-stu-id="2230f-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="2230f-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2230f-115">JSON representation</span></span>
<span data-ttu-id="2230f-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2230f-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sizerange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
