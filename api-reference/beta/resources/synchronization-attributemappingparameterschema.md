---
title: Ressourcentyp attributeMappingParameterSchema
description: Beschreibt einen einzelnen Parameter in einer AttributeMappingFunctionSchema verwendet.
localization_priority: Normal
ms.openlocfilehash: bad88fc58dcc529f086a3e3870e0bb10a9d23329
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529950"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="dc069-103">Ressourcentyp attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="dc069-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc069-104">Beschreibt einen einzelnen Parameter in einer [AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)verwendet.</span><span class="sxs-lookup"><span data-stu-id="dc069-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dc069-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dc069-105">Properties</span></span>

| <span data-ttu-id="dc069-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dc069-106">Property</span></span>                   | <span data-ttu-id="dc069-107">Typ</span><span class="sxs-lookup"><span data-stu-id="dc069-107">Type</span></span>                      | <span data-ttu-id="dc069-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dc069-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="dc069-109">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="dc069-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="dc069-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc069-110">Boolean</span></span>                   |<span data-ttu-id="dc069-111">Der angegebene Parameter kann mehrere Male bereitgestellt werden (beispielsweise Eingabe mehrere Zeichenfolgen der `Concatenate(string,string,...)` Funktion).</span><span class="sxs-lookup"><span data-stu-id="dc069-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="dc069-112">name</span><span class="sxs-lookup"><span data-stu-id="dc069-112">name</span></span>                        |<span data-ttu-id="dc069-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc069-113">String</span></span>                    |<span data-ttu-id="dc069-114">Parametername</span><span class="sxs-lookup"><span data-stu-id="dc069-114">Parameter name.</span></span> |
|<span data-ttu-id="dc069-115">erforderlich</span><span class="sxs-lookup"><span data-stu-id="dc069-115">required</span></span>                    |<span data-ttu-id="dc069-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc069-116">Boolean</span></span>                   |<span data-ttu-id="dc069-117">`true`Wenn der Parameter erforderlich ist. andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="dc069-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="dc069-118">type</span><span class="sxs-lookup"><span data-stu-id="dc069-118">type</span></span>                        |<span data-ttu-id="dc069-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc069-119">String</span></span>                    |<span data-ttu-id="dc069-120">Mögliche Werte: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="dc069-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="dc069-121">Der Standardwert lautet `String`.</span><span class="sxs-lookup"><span data-stu-id="dc069-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc069-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dc069-122">JSON representation</span></span>

<span data-ttu-id="dc069-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dc069-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingparameterschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
