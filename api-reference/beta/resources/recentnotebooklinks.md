---
title: recentNotebookLinks-Ressourcentyp
description: Enthält Links zu einem OneNote-Notizbuch öffnen. Dieser Ressourcentyp ist als Eigenschaft für eine recentNotebook-Ressource vorhanden.
localization_priority: Normal
ms.openlocfilehash: 5ccf861541526a1673d6174176cb8b2a62df6c23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812873"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="c0124-104">recentNotebookLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c0124-104">recentNotebookLinks resource type</span></span>

> <span data-ttu-id="c0124-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0124-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0124-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0124-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0124-107">Enthält Links zu einem OneNote-Notizbuch öffnen.</span><span class="sxs-lookup"><span data-stu-id="c0124-107">Links to open a OneNote notebook.</span></span> <span data-ttu-id="c0124-108">Dieser Ressourcentyp ist als Eigenschaft für eine [recentNotebook](recentnotebook.md)-Ressource vorhanden.</span><span class="sxs-lookup"><span data-stu-id="c0124-108">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="c0124-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c0124-109">Properties</span></span>
| <span data-ttu-id="c0124-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0124-110">Property</span></span>     | <span data-ttu-id="c0124-111">Typ</span><span class="sxs-lookup"><span data-stu-id="c0124-111">Type</span></span>   |<span data-ttu-id="c0124-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0124-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0124-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="c0124-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="c0124-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="c0124-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="c0124-115">Wird das Notizbuch im OneNote-Client geöffnet, wenn es installiert ist.</span><span class="sxs-lookup"><span data-stu-id="c0124-115">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="c0124-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="c0124-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="c0124-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="c0124-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="c0124-118">Öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="c0124-118">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0124-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c0124-119">JSON representation</span></span>

<span data-ttu-id="c0124-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c0124-120">The following is a JSON representation of the resource.</span></span>

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
