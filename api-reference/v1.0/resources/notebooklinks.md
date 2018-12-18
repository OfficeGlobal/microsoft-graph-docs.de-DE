---
title: notebookLinks-Ressourcentyp
description: Links zum Öffnen eines OneNote-Notizbuchs.
author: Jewan-microsoft
ms.openlocfilehash: f263a255199dea844f62d322b4be010111c9c823
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357176"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="3ba44-103">notebookLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3ba44-103">notebookLinks resource type</span></span>

<span data-ttu-id="3ba44-104">Links zum Öffnen eines OneNote-Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="3ba44-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ba44-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3ba44-105">JSON representation</span></span>

<span data-ttu-id="3ba44-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3ba44-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="3ba44-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3ba44-107">Properties</span></span>
| <span data-ttu-id="3ba44-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ba44-108">Property</span></span>     | <span data-ttu-id="3ba44-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3ba44-109">Type</span></span>   |<span data-ttu-id="3ba44-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ba44-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ba44-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="3ba44-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="3ba44-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="3ba44-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="3ba44-113">Öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="3ba44-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="3ba44-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="3ba44-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="3ba44-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="3ba44-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="3ba44-116">Öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="3ba44-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->