---
title: notebookLinks-Ressourcentyp
description: Links zum Öffnen eines OneNote-Notizbuchs.
ms.openlocfilehash: 713779d3bab12222df7a405c1dccb4e6cd4cb235
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017726"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="21bd6-103">notebookLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="21bd6-103">notebookLinks resource type</span></span>

<span data-ttu-id="21bd6-104">Links zum Öffnen eines OneNote-Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="21bd6-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="21bd6-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="21bd6-105">JSON representation</span></span>

<span data-ttu-id="21bd6-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="21bd6-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="21bd6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="21bd6-107">Properties</span></span>
| <span data-ttu-id="21bd6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21bd6-108">Property</span></span>     | <span data-ttu-id="21bd6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="21bd6-109">Type</span></span>   |<span data-ttu-id="21bd6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21bd6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21bd6-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="21bd6-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="21bd6-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="21bd6-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="21bd6-113">Öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="21bd6-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="21bd6-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="21bd6-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="21bd6-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="21bd6-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="21bd6-116">Öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="21bd6-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->