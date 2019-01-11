---
title: notebookLinks-Ressourcentyp
description: Links zum Öffnen eines OneNote-Notizbuchs.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 2666d7da98eeb6115a179ddbbadcd8b5e7f941d7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826883"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="ddbcd-103">notebookLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ddbcd-103">notebookLinks resource type</span></span>

<span data-ttu-id="ddbcd-104">Links zum Öffnen eines OneNote-Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="ddbcd-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddbcd-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ddbcd-105">JSON representation</span></span>

<span data-ttu-id="ddbcd-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ddbcd-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="ddbcd-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ddbcd-107">Properties</span></span>
| <span data-ttu-id="ddbcd-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ddbcd-108">Property</span></span>     | <span data-ttu-id="ddbcd-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ddbcd-109">Type</span></span>   |<span data-ttu-id="ddbcd-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ddbcd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddbcd-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="ddbcd-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="ddbcd-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="ddbcd-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="ddbcd-113">Öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="ddbcd-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="ddbcd-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="ddbcd-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="ddbcd-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="ddbcd-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="ddbcd-116">Öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="ddbcd-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
