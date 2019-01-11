---
title: Zeitstempel Ressourcentyp
description: Datum und Uhrzeit Informationen für einen Punkt in der Zeit.
localization_priority: Normal
ms.openlocfilehash: c63b3bba93f4b108a8eb9943d3fc2a1b2961f06c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888802"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="0965c-103">Zeitstempel Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0965c-103">timeStamp resource type</span></span>

<span data-ttu-id="0965c-104">Datum und Uhrzeit Informationen für einen Punkt in der Zeit.</span><span class="sxs-lookup"><span data-stu-id="0965c-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0965c-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0965c-105">JSON representation</span></span>

<span data-ttu-id="0965c-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0965c-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="0965c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0965c-107">Properties</span></span>
| <span data-ttu-id="0965c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0965c-108">Property</span></span>       | <span data-ttu-id="0965c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0965c-109">Type</span></span>    |<span data-ttu-id="0965c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0965c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0965c-111">date</span><span class="sxs-lookup"><span data-stu-id="0965c-111">date</span></span>|<span data-ttu-id="0965c-112">Datum</span><span class="sxs-lookup"><span data-stu-id="0965c-112">Date</span></span>|<span data-ttu-id="0965c-113">Das der Zeitstempel Datumsteil.</span><span class="sxs-lookup"><span data-stu-id="0965c-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="0965c-114">time</span><span class="sxs-lookup"><span data-stu-id="0965c-114">time</span></span>|<span data-ttu-id="0965c-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0965c-115">TimeOfDay</span></span>|<span data-ttu-id="0965c-116">Den Zeitbereich des der Zeitstempel.</span><span class="sxs-lookup"><span data-stu-id="0965c-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="0965c-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="0965c-117">timeZone</span></span>|<span data-ttu-id="0965c-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0965c-118">String</span></span>|<span data-ttu-id="0965c-119">Der Timezone-Teil der Zeitstempel, der einem der 24 Länge Bereiche in der ganzen Welt ist.</span><span class="sxs-lookup"><span data-stu-id="0965c-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
