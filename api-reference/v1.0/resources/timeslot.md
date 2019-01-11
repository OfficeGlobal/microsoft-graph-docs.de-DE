---
title: Ressourcentyp „timeSlot“
description: Ein Zeitfenster
localization_priority: Normal
ms.openlocfilehash: e01b8d0f34a21eb18bc92e8bcc4e1b8365541d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860564"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="f2639-103">Ressourcentyp „timeSlot“</span><span class="sxs-lookup"><span data-stu-id="f2639-103">timeSlot resource type</span></span>

<span data-ttu-id="f2639-104">Ein Zeitfenster</span><span class="sxs-lookup"><span data-stu-id="f2639-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2639-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f2639-105">JSON representation</span></span>

<span data-ttu-id="f2639-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f2639-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f2639-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f2639-107">Properties</span></span>
| <span data-ttu-id="f2639-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f2639-108">Property</span></span>     | <span data-ttu-id="f2639-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f2639-109">Type</span></span>   |<span data-ttu-id="f2639-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2639-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2639-111">end</span><span class="sxs-lookup"><span data-stu-id="f2639-111">end</span></span>|[<span data-ttu-id="f2639-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f2639-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="f2639-113">Die Startzeit des betreffenden Zeitfensters</span><span class="sxs-lookup"><span data-stu-id="f2639-113">The time a period begins.</span></span>|
|<span data-ttu-id="f2639-114">start</span><span class="sxs-lookup"><span data-stu-id="f2639-114">start</span></span>|[<span data-ttu-id="f2639-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f2639-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="f2639-116">Die Endzeit des betreffenden Zeitfensters</span><span class="sxs-lookup"><span data-stu-id="f2639-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
