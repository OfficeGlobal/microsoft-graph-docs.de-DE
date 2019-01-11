---
title: pageLinks-Ressourcentyp
description: Links zum Öffnen einer OneNote-Seite.
localization_priority: Normal
ms.openlocfilehash: 9bee1b4d3d327118dbf1deec83a37787bd4b18e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832627"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="6d44f-103">pageLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6d44f-103">pageLinks resource type</span></span>

> <span data-ttu-id="6d44f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6d44f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d44f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6d44f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d44f-106">Links zum Öffnen einer OneNote-Seite.</span><span class="sxs-lookup"><span data-stu-id="6d44f-106">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d44f-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6d44f-107">JSON representation</span></span>

<span data-ttu-id="6d44f-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6d44f-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="6d44f-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6d44f-109">Properties</span></span>
| <span data-ttu-id="6d44f-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d44f-110">Property</span></span>     | <span data-ttu-id="6d44f-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6d44f-111">Type</span></span>   |<span data-ttu-id="6d44f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d44f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d44f-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="6d44f-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="6d44f-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="6d44f-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="6d44f-115">Öffnet die Seite im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="6d44f-115">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="6d44f-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="6d44f-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="6d44f-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="6d44f-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="6d44f-118">Öffnet die Seite in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="6d44f-118">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
