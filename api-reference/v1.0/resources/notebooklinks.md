---
title: notebookLinks-Ressourcentyp
description: Links zum Öffnen eines OneNote-Notizbuchs.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d3def81fb9bb3b7f657be3ed04230a65235db5f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984255"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="f7195-103">notebookLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f7195-103">notebookLinks resource type</span></span>

<span data-ttu-id="f7195-104">Links zum Öffnen eines OneNote-Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="f7195-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7195-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f7195-105">JSON representation</span></span>

<span data-ttu-id="f7195-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f7195-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f7195-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f7195-107">Properties</span></span>
| <span data-ttu-id="f7195-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7195-108">Property</span></span>     | <span data-ttu-id="f7195-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f7195-109">Type</span></span>   |<span data-ttu-id="f7195-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7195-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7195-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="f7195-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="f7195-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="f7195-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="f7195-113">Öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="f7195-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="f7195-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="f7195-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="f7195-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="f7195-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="f7195-116">Öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="f7195-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
