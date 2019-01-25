---
title: pageLinks-Ressourcentyp
description: Links zum Öffnen einer OneNote-Seite.
localization_priority: Normal
ms.openlocfilehash: 07c89d99b5731eccd57bec79c25d7d97509c54a0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523827"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="d58c8-103">pageLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d58c8-103">pageLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d58c8-104">Links zum Öffnen einer OneNote-Seite.</span><span class="sxs-lookup"><span data-stu-id="d58c8-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d58c8-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d58c8-105">JSON representation</span></span>

<span data-ttu-id="d58c8-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d58c8-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="d58c8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d58c8-107">Properties</span></span>
| <span data-ttu-id="d58c8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d58c8-108">Property</span></span>     | <span data-ttu-id="d58c8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d58c8-109">Type</span></span>   |<span data-ttu-id="d58c8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d58c8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d58c8-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="d58c8-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="d58c8-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="d58c8-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="d58c8-113">Öffnet die Seite im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="d58c8-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="d58c8-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="d58c8-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="d58c8-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="d58c8-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="d58c8-116">Öffnet die Seite in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="d58c8-116">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/pagelinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
