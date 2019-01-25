---
title: Ressourcentyp stringKeyStringValuePair
description: Ein Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist eine Zeichenfolge, dargestellt.
localization_priority: Normal
ms.openlocfilehash: f91d63ee4b4d3b0328bbb6fbe58c74ec8f78c5b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520221"
---
# <a name="stringkeystringvaluepair-resource-type"></a><span data-ttu-id="f4f21-103">Ressourcentyp stringKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="f4f21-103">stringKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4f21-104">Ein Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist eine Zeichenfolge, dargestellt.</span><span class="sxs-lookup"><span data-stu-id="f4f21-104">Represents a key-value pair where the key is a string and the value is a string.</span></span>

## <a name="properties"></a><span data-ttu-id="f4f21-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f4f21-105">Properties</span></span>
| <span data-ttu-id="f4f21-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f4f21-106">Property</span></span>     | <span data-ttu-id="f4f21-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f4f21-107">Type</span></span>   |<span data-ttu-id="f4f21-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4f21-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4f21-109">Key</span><span class="sxs-lookup"><span data-stu-id="f4f21-109">key</span></span>|<span data-ttu-id="f4f21-110">String</span><span class="sxs-lookup"><span data-stu-id="f4f21-110">String</span></span>|<span data-ttu-id="f4f21-111">Key.</span><span class="sxs-lookup"><span data-stu-id="f4f21-111">Key.</span></span>|
|<span data-ttu-id="f4f21-112">Wert</span><span class="sxs-lookup"><span data-stu-id="f4f21-112">value</span></span>|<span data-ttu-id="f4f21-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4f21-113">String</span></span>|<span data-ttu-id="f4f21-114">Wert.</span><span class="sxs-lookup"><span data-stu-id="f4f21-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4f21-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f4f21-115">JSON representation</span></span>

<span data-ttu-id="f4f21-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f4f21-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeystringvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
