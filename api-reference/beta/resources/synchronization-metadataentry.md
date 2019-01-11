---
title: Ressourcentyp metadataEntry
description: Metadaten für das angegebene Objekt.
localization_priority: Normal
ms.openlocfilehash: ffdb2dd3b6729320b5991b1158e10d145e339968
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819481"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="44b1c-103">Ressourcentyp metadataEntry</span><span class="sxs-lookup"><span data-stu-id="44b1c-103">metadataEntry resource type</span></span>

> <span data-ttu-id="44b1c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="44b1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44b1c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44b1c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44b1c-106">Metadaten für das angegebene Objekt.</span><span class="sxs-lookup"><span data-stu-id="44b1c-106">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="44b1c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="44b1c-107">Properties</span></span>
| <span data-ttu-id="44b1c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="44b1c-108">Property</span></span>     | <span data-ttu-id="44b1c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="44b1c-109">Type</span></span>   |<span data-ttu-id="44b1c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44b1c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44b1c-111">Key</span><span class="sxs-lookup"><span data-stu-id="44b1c-111">key</span></span>|<span data-ttu-id="44b1c-112">String</span><span class="sxs-lookup"><span data-stu-id="44b1c-112">String</span></span>|<span data-ttu-id="44b1c-113">Name der Metadateneigenschaft.</span><span class="sxs-lookup"><span data-stu-id="44b1c-113">Name of the metadata property.</span></span>|
|<span data-ttu-id="44b1c-114">Wert</span><span class="sxs-lookup"><span data-stu-id="44b1c-114">value</span></span>|<span data-ttu-id="44b1c-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="44b1c-115">String</span></span>|<span data-ttu-id="44b1c-116">Der Wert der Metadateneigenschaft.</span><span class="sxs-lookup"><span data-stu-id="44b1c-116">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44b1c-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="44b1c-117">JSON representation</span></span>

<span data-ttu-id="44b1c-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="44b1c-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
