---
title: notebookLinks-Ressourcentyp
description: Links zum Öffnen eines OneNote-Notizbuchs.
author: Jewan-microsoft
ms.openlocfilehash: 88ad146dc4b1499882a2605605c5bb725b6ed531
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345234"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="6094a-103">notebookLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6094a-103">notebookLinks resource type</span></span>

> <span data-ttu-id="6094a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6094a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6094a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6094a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6094a-106">Links zum Öffnen eines OneNote-Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="6094a-106">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6094a-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6094a-107">JSON representation</span></span>

<span data-ttu-id="6094a-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6094a-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="6094a-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6094a-109">Properties</span></span>
| <span data-ttu-id="6094a-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6094a-110">Property</span></span>     | <span data-ttu-id="6094a-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6094a-111">Type</span></span>   |<span data-ttu-id="6094a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6094a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6094a-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="6094a-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="6094a-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="6094a-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="6094a-115">Öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="6094a-115">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="6094a-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="6094a-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="6094a-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="6094a-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="6094a-118">Öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="6094a-118">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->