---
title: Ressourcentyp stringKeyLongValuePair
description: Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist Int64, darstellt.
localization_priority: Normal
ms.openlocfilehash: 97ca9f4f7b4079311a1ce6996fde0472c527e7f9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518303"
---
# <a name="stringkeylongvaluepair-resource-type"></a><span data-ttu-id="5a700-103">Ressourcentyp stringKeyLongValuePair</span><span class="sxs-lookup"><span data-stu-id="5a700-103">stringKeyLongValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a700-104">Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist Int64, darstellt.</span><span class="sxs-lookup"><span data-stu-id="5a700-104">Represents a key-value pair where the key is a string and the value is an Int64.</span></span>

## <a name="properties"></a><span data-ttu-id="5a700-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5a700-105">Properties</span></span>
| <span data-ttu-id="5a700-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5a700-106">Property</span></span>     | <span data-ttu-id="5a700-107">Typ</span><span class="sxs-lookup"><span data-stu-id="5a700-107">Type</span></span>   |<span data-ttu-id="5a700-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a700-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a700-109">Key</span><span class="sxs-lookup"><span data-stu-id="5a700-109">key</span></span>|<span data-ttu-id="5a700-110">String</span><span class="sxs-lookup"><span data-stu-id="5a700-110">String</span></span>|<span data-ttu-id="5a700-111">Key.</span><span class="sxs-lookup"><span data-stu-id="5a700-111">Key.</span></span>|
|<span data-ttu-id="5a700-112">Wert</span><span class="sxs-lookup"><span data-stu-id="5a700-112">value</span></span>|<span data-ttu-id="5a700-113">Int64</span><span class="sxs-lookup"><span data-stu-id="5a700-113">Int64</span></span>|<span data-ttu-id="5a700-114">Wert.</span><span class="sxs-lookup"><span data-stu-id="5a700-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a700-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5a700-115">JSON representation</span></span>

<span data-ttu-id="5a700-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5a700-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyLongValuePair"
}-->

```json
{
  "key": "String",
  "value": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyLongValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeylongvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
