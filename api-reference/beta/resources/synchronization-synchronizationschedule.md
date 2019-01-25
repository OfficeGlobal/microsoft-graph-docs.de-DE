---
title: Ressourcentyp synchronizationSchedule
description: Definiert den Zeitplan zum Ausführen einer SynchronizationJob verwendet.
localization_priority: Normal
ms.openlocfilehash: 0e9714e4833c5586e54c8d812a0d72e41a513e5b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515587"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="7d243-103">Ressourcentyp synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="7d243-103">synchronizationSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d243-104">Definiert den Zeitplan zum Ausführen einer [SynchronizationJob](synchronization-synchronizationjob.md)verwendet.</span><span class="sxs-lookup"><span data-stu-id="7d243-104">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7d243-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7d243-105">Properties</span></span>
| <span data-ttu-id="7d243-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7d243-106">Property</span></span>     | <span data-ttu-id="7d243-107">Typ</span><span class="sxs-lookup"><span data-stu-id="7d243-107">Type</span></span>   |<span data-ttu-id="7d243-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7d243-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d243-109">Ablauf</span><span class="sxs-lookup"><span data-stu-id="7d243-109">expiration</span></span>|<span data-ttu-id="7d243-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d243-110">DateTimeOffset</span></span>|<span data-ttu-id="7d243-111">Datum und Uhrzeit, wann dieser Auftrag abläuft.</span><span class="sxs-lookup"><span data-stu-id="7d243-111">Date and time when this job will expire.</span></span> <span data-ttu-id="7d243-112">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="7d243-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7d243-113">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7d243-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7d243-114">Intervall</span><span class="sxs-lookup"><span data-stu-id="7d243-114">interval</span></span>|<span data-ttu-id="7d243-115">Dauer</span><span class="sxs-lookup"><span data-stu-id="7d243-115">Duration</span></span>|<span data-ttu-id="7d243-116">Das Intervall zwischen Synchronisierung Iterationen.</span><span class="sxs-lookup"><span data-stu-id="7d243-116">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="7d243-117">state</span><span class="sxs-lookup"><span data-stu-id="7d243-117">state</span></span>|<span data-ttu-id="7d243-118">String</span><span class="sxs-lookup"><span data-stu-id="7d243-118">String</span></span>| <span data-ttu-id="7d243-119">Mögliche Werte: `Active`, `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="7d243-119">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d243-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7d243-120">JSON representation</span></span>

<span data-ttu-id="7d243-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7d243-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}-->

```json
{
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
