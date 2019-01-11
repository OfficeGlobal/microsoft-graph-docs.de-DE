---
title: Ressourcentyp „timeSlot“
description: Ein Zeitfenster
localization_priority: Normal
ms.openlocfilehash: 1f383a7feafbb3816ef838d8f0667eebdd42443f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877931"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="5f80b-103">Ressourcentyp „timeSlot“</span><span class="sxs-lookup"><span data-stu-id="5f80b-103">timeSlot resource type</span></span>

> <span data-ttu-id="5f80b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5f80b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f80b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f80b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f80b-106">Ein Zeitfenster</span><span class="sxs-lookup"><span data-stu-id="5f80b-106">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f80b-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5f80b-107">JSON representation</span></span>

<span data-ttu-id="5f80b-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5f80b-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="5f80b-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5f80b-109">Properties</span></span>
| <span data-ttu-id="5f80b-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f80b-110">Property</span></span>     | <span data-ttu-id="5f80b-111">Typ</span><span class="sxs-lookup"><span data-stu-id="5f80b-111">Type</span></span>   |<span data-ttu-id="5f80b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f80b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f80b-113">end</span><span class="sxs-lookup"><span data-stu-id="5f80b-113">end</span></span>|[<span data-ttu-id="5f80b-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5f80b-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="5f80b-115">Die Startzeit des betreffenden Zeitfensters</span><span class="sxs-lookup"><span data-stu-id="5f80b-115">The time a period begins.</span></span>|
|<span data-ttu-id="5f80b-116">start</span><span class="sxs-lookup"><span data-stu-id="5f80b-116">start</span></span>|[<span data-ttu-id="5f80b-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5f80b-117">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="5f80b-118">Die Endzeit des betreffenden Zeitfensters</span><span class="sxs-lookup"><span data-stu-id="5f80b-118">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
