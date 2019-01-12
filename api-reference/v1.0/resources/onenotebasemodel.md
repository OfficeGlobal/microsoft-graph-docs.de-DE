---
title: OnenoteEntityBaseModel-Ressource
description: Dies ist der Basistyp für OneNote-Entitäten.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 53ed86ae22f3ac9fccdef98e56382cd9440e71e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923131"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="bd9c2-103">OnenoteEntityBaseModel-Ressource</span><span class="sxs-lookup"><span data-stu-id="bd9c2-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="bd9c2-104">Dies ist der Basistyp für OneNote-Entitäten.</span><span class="sxs-lookup"><span data-stu-id="bd9c2-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd9c2-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd9c2-105">JSON representation</span></span>

<span data-ttu-id="bd9c2-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd9c2-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="bd9c2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd9c2-107">Properties</span></span>
| <span data-ttu-id="bd9c2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd9c2-108">Property</span></span>     | <span data-ttu-id="bd9c2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bd9c2-109">Type</span></span>   |<span data-ttu-id="bd9c2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd9c2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd9c2-111">self</span><span class="sxs-lookup"><span data-stu-id="bd9c2-111">self</span></span>|<span data-ttu-id="bd9c2-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd9c2-112">String</span></span>|<span data-ttu-id="bd9c2-p101">Der Endpunkt, an dem Sie Details zur Seite abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bd9c2-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
