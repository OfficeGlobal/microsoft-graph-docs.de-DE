---
title: notebookLinks-Ressourcentyp
description: Links zum Öffnen eines OneNote-Notizbuchs.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: f6995c112410d22cfe5849f54d0077bf8b79f6b3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517365"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="ba398-103">notebookLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ba398-103">notebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba398-104">Links zum Öffnen eines OneNote-Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="ba398-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba398-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ba398-105">JSON representation</span></span>

<span data-ttu-id="ba398-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ba398-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ba398-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ba398-107">Properties</span></span>
| <span data-ttu-id="ba398-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ba398-108">Property</span></span>     | <span data-ttu-id="ba398-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ba398-109">Type</span></span>   |<span data-ttu-id="ba398-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba398-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba398-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="ba398-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="ba398-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="ba398-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="ba398-113">Öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="ba398-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="ba398-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="ba398-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="ba398-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="ba398-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="ba398-116">Öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="ba398-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/notebooklinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
