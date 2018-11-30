---
title: Ressourcentyp metadataEntry
description: Metadaten für das angegebene Objekt.
ms.openlocfilehash: 8fed980c5310b0a9f13a6f3269dde90fad083751
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058927"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="9ceb1-103">Ressourcentyp metadataEntry</span><span class="sxs-lookup"><span data-stu-id="9ceb1-103">metadataEntry resource type</span></span>

> <span data-ttu-id="9ceb1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9ceb1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ceb1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ceb1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ceb1-106">Metadaten für das angegebene Objekt.</span><span class="sxs-lookup"><span data-stu-id="9ceb1-106">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="9ceb1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9ceb1-107">Properties</span></span>
| <span data-ttu-id="9ceb1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ceb1-108">Property</span></span>     | <span data-ttu-id="9ceb1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9ceb1-109">Type</span></span>   |<span data-ttu-id="9ceb1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ceb1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ceb1-111">Key</span><span class="sxs-lookup"><span data-stu-id="9ceb1-111">key</span></span>|<span data-ttu-id="9ceb1-112">String</span><span class="sxs-lookup"><span data-stu-id="9ceb1-112">String</span></span>|<span data-ttu-id="9ceb1-113">Name der Metadateneigenschaft.</span><span class="sxs-lookup"><span data-stu-id="9ceb1-113">Name of the metadata property.</span></span>|
|<span data-ttu-id="9ceb1-114">Wert</span><span class="sxs-lookup"><span data-stu-id="9ceb1-114">value</span></span>|<span data-ttu-id="9ceb1-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ceb1-115">String</span></span>|<span data-ttu-id="9ceb1-116">Der Wert der Metadateneigenschaft.</span><span class="sxs-lookup"><span data-stu-id="9ceb1-116">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ceb1-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9ceb1-117">JSON representation</span></span>

<span data-ttu-id="9ceb1-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9ceb1-118">The following is a JSON representation of the resource.</span></span>

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