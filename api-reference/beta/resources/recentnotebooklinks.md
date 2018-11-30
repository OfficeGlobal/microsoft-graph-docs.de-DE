---
title: recentNotebookLinks-Ressourcentyp
description: Enthält Links zu einem OneNote-Notizbuch öffnen. Dieser Ressourcentyp ist als Eigenschaft für eine recentNotebook-Ressource vorhanden.
ms.openlocfilehash: de13f25148425a1816a60f6cf5b9f4a09f61c7dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061728"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="d18fe-104">recentNotebookLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d18fe-104">recentNotebookLinks resource type</span></span>

> <span data-ttu-id="d18fe-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d18fe-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d18fe-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d18fe-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d18fe-107">Enthält Links zu einem OneNote-Notizbuch öffnen.</span><span class="sxs-lookup"><span data-stu-id="d18fe-107">Links to open a OneNote notebook.</span></span> <span data-ttu-id="d18fe-108">Dieser Ressourcentyp ist als Eigenschaft für eine [recentNotebook](recentnotebook.md)-Ressource vorhanden.</span><span class="sxs-lookup"><span data-stu-id="d18fe-108">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d18fe-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d18fe-109">Properties</span></span>
| <span data-ttu-id="d18fe-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d18fe-110">Property</span></span>     | <span data-ttu-id="d18fe-111">Typ</span><span class="sxs-lookup"><span data-stu-id="d18fe-111">Type</span></span>   |<span data-ttu-id="d18fe-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d18fe-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d18fe-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="d18fe-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="d18fe-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="d18fe-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="d18fe-115">Wird das Notizbuch im OneNote-Client geöffnet, wenn es installiert ist.</span><span class="sxs-lookup"><span data-stu-id="d18fe-115">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="d18fe-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="d18fe-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="d18fe-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="d18fe-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="d18fe-118">Öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="d18fe-118">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d18fe-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d18fe-119">JSON representation</span></span>

<span data-ttu-id="d18fe-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d18fe-120">The following is a JSON representation of the resource.</span></span>

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
