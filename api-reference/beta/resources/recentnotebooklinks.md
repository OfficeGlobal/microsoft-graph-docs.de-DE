---
title: recentNotebookLinks-Ressourcentyp
description: Enthält Links zu einem OneNote-Notizbuch öffnen. Dieser Ressourcentyp ist als Eigenschaft für eine recentNotebook-Ressource vorhanden.
localization_priority: Normal
ms.openlocfilehash: 328f337d63645cdd52722a4216006920c493f9e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525885"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="bfc1d-104">recentNotebookLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bfc1d-104">recentNotebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfc1d-105">Enthält Links zu einem OneNote-Notizbuch öffnen.</span><span class="sxs-lookup"><span data-stu-id="bfc1d-105">Links to open a OneNote notebook.</span></span> <span data-ttu-id="bfc1d-106">Dieser Ressourcentyp ist als Eigenschaft für eine [recentNotebook](recentnotebook.md)-Ressource vorhanden.</span><span class="sxs-lookup"><span data-stu-id="bfc1d-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="bfc1d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bfc1d-107">Properties</span></span>
| <span data-ttu-id="bfc1d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bfc1d-108">Property</span></span>     | <span data-ttu-id="bfc1d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bfc1d-109">Type</span></span>   |<span data-ttu-id="bfc1d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfc1d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfc1d-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="bfc1d-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="bfc1d-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="bfc1d-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="bfc1d-113">Wird das Notizbuch im OneNote-Client geöffnet, wenn es installiert ist.</span><span class="sxs-lookup"><span data-stu-id="bfc1d-113">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="bfc1d-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="bfc1d-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="bfc1d-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="bfc1d-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="bfc1d-116">Öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="bfc1d-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfc1d-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bfc1d-117">JSON representation</span></span>

<span data-ttu-id="bfc1d-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bfc1d-118">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/recentnotebooklinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
