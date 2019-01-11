---
title: sectionLinks-Ressourcentyp
description: Links zum Öffnen eines OneNote-Abschnitts.
localization_priority: Normal
ms.openlocfilehash: afc740aebc494aa6f204febbce1be4433005a4b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839935"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="9f090-103">sectionLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9f090-103">sectionLinks resource type</span></span>

<span data-ttu-id="9f090-104">Links zum Öffnen eines OneNote-Abschnitts.</span><span class="sxs-lookup"><span data-stu-id="9f090-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f090-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9f090-105">JSON representation</span></span>

<span data-ttu-id="9f090-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9f090-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="9f090-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9f090-107">Properties</span></span>
| <span data-ttu-id="9f090-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9f090-108">Property</span></span>     | <span data-ttu-id="9f090-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9f090-109">Type</span></span>   |<span data-ttu-id="9f090-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f090-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f090-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="9f090-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="9f090-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="9f090-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="9f090-113">Öffnet den Abschnitt im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="9f090-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="9f090-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="9f090-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="9f090-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="9f090-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="9f090-116">Öffnet den Abschnitt in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="9f090-116">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
