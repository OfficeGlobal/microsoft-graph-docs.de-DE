---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.openlocfilehash: f7293b986b5e6d77d0601cffb6b60edc5dfd2dd7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856028"
---
# <a name="webpart-resource"></a><span data-ttu-id="bbf96-102">WebPart-Ressource</span><span class="sxs-lookup"><span data-stu-id="bbf96-102">webPart resource</span></span>

> <span data-ttu-id="bbf96-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bbf96-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbf96-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bbf96-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bbf96-105">Die **WebPart** -Ressource stellt Typ und von Renderinginformationen für ein Webpart auf einer [SitePage](sitepage.md)dar.</span><span class="sxs-lookup"><span data-stu-id="bbf96-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbf96-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bbf96-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="bbf96-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bbf96-107">Properties</span></span>

| <span data-ttu-id="bbf96-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bbf96-108">Property</span></span>                | <span data-ttu-id="bbf96-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bbf96-109">Type</span></span>             | <span data-ttu-id="bbf96-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbf96-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="bbf96-111">**type**</span><span class="sxs-lookup"><span data-stu-id="bbf96-111">**type**</span></span>                | <span data-ttu-id="bbf96-112">String</span><span class="sxs-lookup"><span data-stu-id="bbf96-112">String</span></span>           | <span data-ttu-id="bbf96-113">Ein eindeutiger Bezeichner, der den WebPart angibt.</span><span class="sxs-lookup"><span data-stu-id="bbf96-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="bbf96-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bbf96-114">Read-only.</span></span>
| <span data-ttu-id="bbf96-115">**data**</span><span class="sxs-lookup"><span data-stu-id="bbf96-115">**data**</span></span>                | <span data-ttu-id="bbf96-116">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="bbf96-116">[sitePageData][]</span></span> | <span data-ttu-id="bbf96-117">Die erforderlichen Eigenschaften für das WebPart (hängt vom WebPart)</span><span class="sxs-lookup"><span data-stu-id="bbf96-117">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="bbf96-119">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="bbf96-119">Remarks</span></span>

<span data-ttu-id="bbf96-120">Webparts können ihre eigenen erforderlichen Eigenschaften unter **Daten**definieren.</span><span class="sxs-lookup"><span data-stu-id="bbf96-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="bbf96-121">Weitere Informationen zu Seiten finden Sie unter [SitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="bbf96-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->
