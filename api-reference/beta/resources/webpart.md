---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e7bbd0f6aa8d4ea04304d6aecae97b98ab0a46b7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574278"
---
# <a name="webpart-resource"></a><span data-ttu-id="77891-102">WebPart-Ressource</span><span class="sxs-lookup"><span data-stu-id="77891-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77891-103">Die **WebPart** -Ressource stellt Typ und von Renderinginformationen für ein Webpart auf einer [SitePage](sitepage.md)dar.</span><span class="sxs-lookup"><span data-stu-id="77891-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="77891-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77891-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  
    ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "String (identifier)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a><span data-ttu-id="77891-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77891-105">Properties</span></span>

| <span data-ttu-id="77891-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77891-106">Property</span></span>                | <span data-ttu-id="77891-107">Typ</span><span class="sxs-lookup"><span data-stu-id="77891-107">Type</span></span>             | <span data-ttu-id="77891-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77891-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="77891-109">**type**</span><span class="sxs-lookup"><span data-stu-id="77891-109">**type**</span></span>                | <span data-ttu-id="77891-110">Zeichenfolge (ID)</span><span class="sxs-lookup"><span data-stu-id="77891-110">String (identifier)</span></span>         | <span data-ttu-id="77891-111">Ein eindeutiger Bezeichner, der den WebPart angibt.</span><span class="sxs-lookup"><span data-stu-id="77891-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="77891-112">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="77891-112">Read-only.</span></span>
| <span data-ttu-id="77891-113">**data**</span><span class="sxs-lookup"><span data-stu-id="77891-113">**data**</span></span>                | [<span data-ttu-id="77891-114">sitePageData</span><span class="sxs-lookup"><span data-stu-id="77891-114">sitePageData</span></span>](sitepagedata.md) | <span data-ttu-id="77891-115">Die erforderlichen Eigenschaften für das WebPart (hängt vom WebPart)</span><span class="sxs-lookup"><span data-stu-id="77891-115">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="77891-116">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="77891-116">Remarks</span></span>

<span data-ttu-id="77891-117">Webparts können ihre eigenen erforderlichen Eigenschaften unter **Daten**definieren.</span><span class="sxs-lookup"><span data-stu-id="77891-117">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="77891-118">Weitere Informationen zu Seiten finden Sie unter [SitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="77891-118">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
