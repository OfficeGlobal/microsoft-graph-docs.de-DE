---
title: Ressourcentyp attributeMappingParameterSchema
description: Beschreibt einen einzelnen Parameter in einer AttributeMappingFunctionSchema verwendet.
ms.openlocfilehash: 164387a345f245f390d24b89a349e02ee2242041
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064838"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="8c997-103">Ressourcentyp attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="8c997-103">attributeMappingParameterSchema resource type</span></span>

> <span data-ttu-id="8c997-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8c997-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c997-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c997-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c997-106">Beschreibt einen einzelnen Parameter in einer [AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)verwendet.</span><span class="sxs-lookup"><span data-stu-id="8c997-106">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8c997-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8c997-107">Properties</span></span>

| <span data-ttu-id="8c997-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8c997-108">Property</span></span>                   | <span data-ttu-id="8c997-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8c997-109">Type</span></span>                      | <span data-ttu-id="8c997-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c997-110">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="8c997-111">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="8c997-111">allowMultipleOccurrences</span></span>    |<span data-ttu-id="8c997-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8c997-112">Boolean</span></span>                   |<span data-ttu-id="8c997-113">Der angegebene Parameter kann mehrere Male bereitgestellt werden (beispielsweise Eingabe mehrere Zeichenfolgen der `Concatenate(string,string,...)` Funktion).</span><span class="sxs-lookup"><span data-stu-id="8c997-113">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="8c997-114">name</span><span class="sxs-lookup"><span data-stu-id="8c997-114">name</span></span>                        |<span data-ttu-id="8c997-115">String</span><span class="sxs-lookup"><span data-stu-id="8c997-115">String</span></span>                    |<span data-ttu-id="8c997-116">Name des Parameters.</span><span class="sxs-lookup"><span data-stu-id="8c997-116">Parameter name.</span></span> |
|<span data-ttu-id="8c997-117">erforderlich</span><span class="sxs-lookup"><span data-stu-id="8c997-117">required</span></span>                    |<span data-ttu-id="8c997-118">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8c997-118">Boolean</span></span>                   |<span data-ttu-id="8c997-119">`true`Wenn der Parameter erforderlich ist. andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="8c997-119">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="8c997-120">Typ</span><span class="sxs-lookup"><span data-stu-id="8c997-120">type</span></span>                        |<span data-ttu-id="8c997-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8c997-121">String</span></span>                    |<span data-ttu-id="8c997-122">Mögliche Werte: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="8c997-122">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="8c997-123">Der Standardwert lautet `String`.</span><span class="sxs-lookup"><span data-stu-id="8c997-123">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c997-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8c997-124">JSON representation</span></span>

<span data-ttu-id="8c997-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8c997-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->