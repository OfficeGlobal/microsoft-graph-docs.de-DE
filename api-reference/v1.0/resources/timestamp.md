---
title: Zeitstempel Ressourcentyp
description: Datum und Uhrzeit Informationen für einen Punkt in der Zeit.
ms.openlocfilehash: 4f392e880bb165841fd8a9a31b6ed00bf2ba36fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016744"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="47c45-103">Zeitstempel Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="47c45-103">timeStamp resource type</span></span>

<span data-ttu-id="47c45-104">Datum und Uhrzeit Informationen für einen Punkt in der Zeit.</span><span class="sxs-lookup"><span data-stu-id="47c45-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="47c45-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="47c45-105">JSON representation</span></span>

<span data-ttu-id="47c45-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="47c45-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="47c45-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="47c45-107">Properties</span></span>
| <span data-ttu-id="47c45-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="47c45-108">Property</span></span>       | <span data-ttu-id="47c45-109">Typ</span><span class="sxs-lookup"><span data-stu-id="47c45-109">Type</span></span>    |<span data-ttu-id="47c45-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="47c45-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47c45-111">date</span><span class="sxs-lookup"><span data-stu-id="47c45-111">date</span></span>|<span data-ttu-id="47c45-112">Datum</span><span class="sxs-lookup"><span data-stu-id="47c45-112">Date</span></span>|<span data-ttu-id="47c45-113">Das der Zeitstempel Datumsteil.</span><span class="sxs-lookup"><span data-stu-id="47c45-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="47c45-114">time</span><span class="sxs-lookup"><span data-stu-id="47c45-114">time</span></span>|<span data-ttu-id="47c45-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="47c45-115">TimeOfDay</span></span>|<span data-ttu-id="47c45-116">Den Zeitbereich des der Zeitstempel.</span><span class="sxs-lookup"><span data-stu-id="47c45-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="47c45-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="47c45-117">timeZone</span></span>|<span data-ttu-id="47c45-118">String</span><span class="sxs-lookup"><span data-stu-id="47c45-118">String</span></span>|<span data-ttu-id="47c45-119">Der Timezone-Teil der Zeitstempel, der einem der 24 Länge Bereiche in der ganzen Welt ist.</span><span class="sxs-lookup"><span data-stu-id="47c45-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->