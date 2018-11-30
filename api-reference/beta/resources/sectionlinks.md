---
title: sectionLinks-Ressourcentyp
description: Links zum Öffnen eines OneNote-Abschnitts.
ms.openlocfilehash: 26dbffd6f3bde9c05efabc737852c3619cc1e275
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063464"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="e5f06-103">sectionLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e5f06-103">sectionLinks resource type</span></span>

> <span data-ttu-id="e5f06-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e5f06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5f06-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5f06-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5f06-106">Links zum Öffnen eines OneNote-Abschnitts.</span><span class="sxs-lookup"><span data-stu-id="e5f06-106">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5f06-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e5f06-107">JSON representation</span></span>

<span data-ttu-id="e5f06-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e5f06-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e5f06-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e5f06-109">Properties</span></span>
| <span data-ttu-id="e5f06-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e5f06-110">Property</span></span>     | <span data-ttu-id="e5f06-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e5f06-111">Type</span></span>   |<span data-ttu-id="e5f06-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5f06-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5f06-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="e5f06-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="e5f06-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="e5f06-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="e5f06-115">Öffnet den Abschnitt im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="e5f06-115">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="e5f06-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="e5f06-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="e5f06-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="e5f06-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="e5f06-118">Öffnet den Abschnitt in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="e5f06-118">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->