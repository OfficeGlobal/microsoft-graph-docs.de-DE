---
title: Ressourcentyp „timeSlot“
description: Ein Zeitfenster
ms.openlocfilehash: c1df6ea458bf6742dc20149e62d9760a8a6510e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064805"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="00c6b-103">Ressourcentyp „timeSlot“</span><span class="sxs-lookup"><span data-stu-id="00c6b-103">timeSlot resource type</span></span>

> <span data-ttu-id="00c6b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="00c6b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00c6b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00c6b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00c6b-106">Ein Zeitfenster</span><span class="sxs-lookup"><span data-stu-id="00c6b-106">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="00c6b-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="00c6b-107">JSON representation</span></span>

<span data-ttu-id="00c6b-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="00c6b-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="00c6b-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="00c6b-109">Properties</span></span>
| <span data-ttu-id="00c6b-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00c6b-110">Property</span></span>     | <span data-ttu-id="00c6b-111">Typ</span><span class="sxs-lookup"><span data-stu-id="00c6b-111">Type</span></span>   |<span data-ttu-id="00c6b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00c6b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00c6b-113">end</span><span class="sxs-lookup"><span data-stu-id="00c6b-113">end</span></span>|[<span data-ttu-id="00c6b-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="00c6b-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="00c6b-115">Die Startzeit des betreffenden Zeitfensters</span><span class="sxs-lookup"><span data-stu-id="00c6b-115">The time a period begins.</span></span>|
|<span data-ttu-id="00c6b-116">start</span><span class="sxs-lookup"><span data-stu-id="00c6b-116">start</span></span>|[<span data-ttu-id="00c6b-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="00c6b-117">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="00c6b-118">Die Endzeit des betreffenden Zeitfensters</span><span class="sxs-lookup"><span data-stu-id="00c6b-118">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->