---
title: recentNotebookLinks-Ressourcentyp
description: Links zum Öffnen eines OneNote-Notizbuchs. Dieser Ressourcentyp ist als Eigenschaft für eine recentNotebook-Ressource vorhanden.
localization_priority: Normal
ms.openlocfilehash: 846047bd602d19cb4745e0a63f0326aaf7bfb512
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810584"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="49273-104">recentNotebookLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="49273-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="49273-105">Links zum Öffnen eines OneNote-Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="49273-105">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="49273-106">Dieser Ressourcentyp ist als Eigenschaft für eine [recentNotebook](recentnotebook.md)-Ressource vorhanden.</span><span class="sxs-lookup"><span data-stu-id="49273-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="49273-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="49273-107">Properties</span></span>
| <span data-ttu-id="49273-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49273-108">Property</span></span>     | <span data-ttu-id="49273-109">Typ</span><span class="sxs-lookup"><span data-stu-id="49273-109">Type</span></span>   |<span data-ttu-id="49273-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49273-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49273-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="49273-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="49273-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="49273-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="49273-113">Öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="49273-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="49273-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="49273-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="49273-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="49273-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="49273-116">Öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="49273-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49273-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="49273-117">JSON representation</span></span>

<span data-ttu-id="49273-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="49273-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
