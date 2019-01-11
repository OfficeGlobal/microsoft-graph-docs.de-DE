---
title: OnenoteEntityBaseModel-Ressource
description: Dies ist der Basistyp für OneNote-Entitäten.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 0c6a3d4916bf54eeec5856f51af87fa79e1f6e6c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821231"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="e0796-103">OnenoteEntityBaseModel-Ressource</span><span class="sxs-lookup"><span data-stu-id="e0796-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="e0796-104">Dies ist der Basistyp für OneNote-Entitäten.</span><span class="sxs-lookup"><span data-stu-id="e0796-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0796-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e0796-105">JSON representation</span></span>

<span data-ttu-id="e0796-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e0796-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityBaseModel"
}-->

```json
{
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e0796-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e0796-107">Properties</span></span>
| <span data-ttu-id="e0796-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e0796-108">Property</span></span>     | <span data-ttu-id="e0796-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e0796-109">Type</span></span>   |<span data-ttu-id="e0796-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0796-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0796-111">self</span><span class="sxs-lookup"><span data-stu-id="e0796-111">self</span></span>|<span data-ttu-id="e0796-112">String</span><span class="sxs-lookup"><span data-stu-id="e0796-112">String</span></span>|<span data-ttu-id="e0796-p101">Der Endpunkt, an dem Sie Details zur Seite abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e0796-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
