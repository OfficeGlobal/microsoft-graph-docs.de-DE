---
title: pageLinks-Ressourcentyp
description: Links zum Öffnen einer OneNote-Seite.
ms.openlocfilehash: f1e4fe36d4356986bc88b744a9a62e28b8d368c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016575"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="0983e-103">pageLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0983e-103">pageLinks resource type</span></span>

<span data-ttu-id="0983e-104">Links zum Öffnen einer OneNote-Seite.</span><span class="sxs-lookup"><span data-stu-id="0983e-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0983e-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0983e-105">JSON representation</span></span>

<span data-ttu-id="0983e-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0983e-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pageLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="0983e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0983e-107">Properties</span></span>
| <span data-ttu-id="0983e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0983e-108">Property</span></span>     | <span data-ttu-id="0983e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0983e-109">Type</span></span>   |<span data-ttu-id="0983e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0983e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0983e-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="0983e-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="0983e-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="0983e-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="0983e-113">Öffnet die Seite im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="0983e-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="0983e-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="0983e-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="0983e-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="0983e-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="0983e-116">Öffnet die Seite in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="0983e-116">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->