---
title: OnenoteEntityBaseModel-Ressource
description: Dies ist der Basistyp für OneNote-Entitäten.
author: Jewan-microsoft
ms.openlocfilehash: 25e2da6732fd831c6bbec5ae86bddeae7b702aa5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310465"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="0800f-103">OnenoteEntityBaseModel-Ressource</span><span class="sxs-lookup"><span data-stu-id="0800f-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="0800f-104">Dies ist der Basistyp für OneNote-Entitäten.</span><span class="sxs-lookup"><span data-stu-id="0800f-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0800f-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0800f-105">JSON representation</span></span>

<span data-ttu-id="0800f-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0800f-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0800f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0800f-107">Properties</span></span>
| <span data-ttu-id="0800f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0800f-108">Property</span></span>     | <span data-ttu-id="0800f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0800f-109">Type</span></span>   |<span data-ttu-id="0800f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0800f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0800f-111">self</span><span class="sxs-lookup"><span data-stu-id="0800f-111">self</span></span>|<span data-ttu-id="0800f-112">String</span><span class="sxs-lookup"><span data-stu-id="0800f-112">String</span></span>|<span data-ttu-id="0800f-p101">Der Endpunkt, an dem Sie Details zur Seite abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0800f-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->