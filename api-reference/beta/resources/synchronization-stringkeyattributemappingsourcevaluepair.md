---
title: Ressourcentyp stringKeyAttributeMappingSourceValuePair
description: Stellt ein Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist AttributeMappingSource.
ms.openlocfilehash: 875c593ae652ce763f420d29e5dd4e5e2601bc88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065195"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="768c7-103">Ressourcentyp stringKeyAttributeMappingSourceValuePair</span><span class="sxs-lookup"><span data-stu-id="768c7-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

> <span data-ttu-id="768c7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="768c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="768c7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="768c7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="768c7-106">Stellt ein Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist [AttributeMappingSource](synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="768c7-106">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="768c7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="768c7-107">Properties</span></span>
| <span data-ttu-id="768c7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="768c7-108">Property</span></span>     | <span data-ttu-id="768c7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="768c7-109">Type</span></span>   |<span data-ttu-id="768c7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="768c7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="768c7-111">Key</span><span class="sxs-lookup"><span data-stu-id="768c7-111">key</span></span>|<span data-ttu-id="768c7-112">String</span><span class="sxs-lookup"><span data-stu-id="768c7-112">String</span></span>|<span data-ttu-id="768c7-113">Der Name des Parameters.</span><span class="sxs-lookup"><span data-stu-id="768c7-113">The name of the parameter.</span></span>|
|<span data-ttu-id="768c7-114">Wert</span><span class="sxs-lookup"><span data-stu-id="768c7-114">value</span></span>|[<span data-ttu-id="768c7-115">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="768c7-115">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="768c7-116">Der Wert des Parameters.</span><span class="sxs-lookup"><span data-stu-id="768c7-116">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="768c7-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="768c7-117">JSON representation</span></span>

<span data-ttu-id="768c7-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="768c7-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
