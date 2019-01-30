---
title: Ressourcentyp stringKeyObjectValuePair
description: Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist ein beliebiges JSON-Objekt, darstellt. Dies ist ein open OData-Typ, die eine Eigenschaft mit dem Namen haben erwartet `value` also ein gültiges JSON-Objekt.
localization_priority: Normal
ms.openlocfilehash: 8f939c177f2130813c6080d46ad78664f6118857
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642926"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="ae87a-104">Ressourcentyp stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="ae87a-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae87a-105">Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist ein beliebiges JSON-Objekt, darstellt.</span><span class="sxs-lookup"><span data-stu-id="ae87a-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="ae87a-106">Dies ist ein open OData-Typ, die eine Eigenschaft mit dem Namen haben erwartet `value` also ein gültiges JSON-Objekt.</span><span class="sxs-lookup"><span data-stu-id="ae87a-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="ae87a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ae87a-107">Properties</span></span>
| <span data-ttu-id="ae87a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae87a-108">Property</span></span>     | <span data-ttu-id="ae87a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ae87a-109">Type</span></span>   |<span data-ttu-id="ae87a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae87a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae87a-111">Key</span><span class="sxs-lookup"><span data-stu-id="ae87a-111">key</span></span>|<span data-ttu-id="ae87a-112">String</span><span class="sxs-lookup"><span data-stu-id="ae87a-112">String</span></span>|<span data-ttu-id="ae87a-113">Key.</span><span class="sxs-lookup"><span data-stu-id="ae87a-113">Key.</span></span>|
|<span data-ttu-id="ae87a-114">Wert</span><span class="sxs-lookup"><span data-stu-id="ae87a-114">value</span></span>|<span data-ttu-id="ae87a-115">Jede</span><span class="sxs-lookup"><span data-stu-id="ae87a-115">Any</span></span>|<span data-ttu-id="ae87a-116">Beliebige JSON-Objekt.</span><span class="sxs-lookup"><span data-stu-id="ae87a-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae87a-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ae87a-117">JSON representation</span></span>

<span data-ttu-id="ae87a-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ae87a-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeyobjectvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
