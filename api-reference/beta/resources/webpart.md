---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640175"
---
# <a name="webpart-resource"></a><span data-ttu-id="46926-102">WebPart-Ressource</span><span class="sxs-lookup"><span data-stu-id="46926-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46926-103">Die **WebPart** -Ressource stellt Typ und von Renderinginformationen für ein Webpart auf einer [SitePage](sitepage.md)dar.</span><span class="sxs-lookup"><span data-stu-id="46926-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="46926-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="46926-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a><span data-ttu-id="46926-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="46926-105">Properties</span></span>

| <span data-ttu-id="46926-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46926-106">Property</span></span>                | <span data-ttu-id="46926-107">Typ</span><span class="sxs-lookup"><span data-stu-id="46926-107">Type</span></span>             | <span data-ttu-id="46926-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46926-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="46926-109">**type**</span><span class="sxs-lookup"><span data-stu-id="46926-109">**type**</span></span>                | <span data-ttu-id="46926-110">String</span><span class="sxs-lookup"><span data-stu-id="46926-110">String</span></span>           | <span data-ttu-id="46926-111">Ein eindeutiger Bezeichner, der den WebPart angibt.</span><span class="sxs-lookup"><span data-stu-id="46926-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="46926-112">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="46926-112">Read-only.</span></span>
| <span data-ttu-id="46926-113">**data**</span><span class="sxs-lookup"><span data-stu-id="46926-113">**data**</span></span>                | <span data-ttu-id="46926-114">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="46926-114">[sitePageData][]</span></span> | <span data-ttu-id="46926-115">Die erforderlichen Eigenschaften für das WebPart (hängt vom WebPart)</span><span class="sxs-lookup"><span data-stu-id="46926-115">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="46926-117">Hinweise</span><span class="sxs-lookup"><span data-stu-id="46926-117">Remarks</span></span>

<span data-ttu-id="46926-118">Webparts können ihre eigenen erforderlichen Eigenschaften unter **Daten**definieren.</span><span class="sxs-lookup"><span data-stu-id="46926-118">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="46926-119">Weitere Informationen zu Seiten finden Sie unter [SitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="46926-119">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": [
    "Error: /api-reference/beta/resources/webpart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
