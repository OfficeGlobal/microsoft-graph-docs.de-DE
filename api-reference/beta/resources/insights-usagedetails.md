---
title: Ressourcentyp usageDetails
description: Komplexer Typ, die Eigenschaften des verwendeten Elemente enthält. Wenn die Ressource des letzten Zugriffs auf Informationen (Ansicht) und (bearbeitet) vom Benutzer geändert.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 04e064d5ebf8599466218722d89f46ececc5e58c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577487"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="08d39-104">Ressourcentyp usageDetails</span><span class="sxs-lookup"><span data-stu-id="08d39-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08d39-105">Komplexer Typ, enthält die Eigenschaften von Elementen [verwendet](insights-used.md) .</span><span class="sxs-lookup"><span data-stu-id="08d39-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="08d39-106">Wenn die Ressource des letzten Zugriffs auf Informationen (Ansicht) und (bearbeitet) vom Benutzer geändert.</span><span class="sxs-lookup"><span data-stu-id="08d39-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="08d39-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08d39-107">JSON representation</span></span>

<span data-ttu-id="08d39-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08d39-108">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usageDetails"
}-->
```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="08d39-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08d39-109">Properties</span></span>

| <span data-ttu-id="08d39-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08d39-110">Property</span></span>              | <span data-ttu-id="08d39-111">Typ</span><span class="sxs-lookup"><span data-stu-id="08d39-111">Type</span></span>          | <span data-ttu-id="08d39-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08d39-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="08d39-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="08d39-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="08d39-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08d39-114">DateTimeOffset</span></span>        | <span data-ttu-id="08d39-115">Das Datum und die Zeit, die die Ressource zuletzt vom Benutzer zugegriffen werden konnte.</span><span class="sxs-lookup"><span data-stu-id="08d39-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="08d39-116">Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="08d39-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="08d39-117">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="08d39-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="08d39-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="08d39-118">Read-only.</span></span>                      |
| <span data-ttu-id="08d39-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08d39-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="08d39-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08d39-120">DateTimeOffset</span></span>        | <span data-ttu-id="08d39-121">Datum und Uhrzeit der letzten Änderung die Ressource durch den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="08d39-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="08d39-122">Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="08d39-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="08d39-123">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="08d39-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="08d39-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="08d39-124">Read-only.</span></span>       |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-usagedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
