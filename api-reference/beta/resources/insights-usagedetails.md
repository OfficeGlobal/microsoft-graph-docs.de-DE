---
title: Ressourcentyp usageDetails
description: Komplexer Typ, die Eigenschaften des verwendeten Elemente enthält. Wenn die Ressource des letzten Zugriffs auf Informationen (Ansicht) und (bearbeitet) vom Benutzer geändert.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4df15bf635785aba054d52beb89b5ac04d48d3d3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526830"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="0a8d5-104">Ressourcentyp usageDetails</span><span class="sxs-lookup"><span data-stu-id="0a8d5-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a8d5-105">Komplexer Typ, enthält die Eigenschaften von Elementen [verwendet](insights-used.md) .</span><span class="sxs-lookup"><span data-stu-id="0a8d5-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="0a8d5-106">Wenn die Ressource des letzten Zugriffs auf Informationen (Ansicht) und (bearbeitet) vom Benutzer geändert.</span><span class="sxs-lookup"><span data-stu-id="0a8d5-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a8d5-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0a8d5-107">JSON representation</span></span>

<span data-ttu-id="0a8d5-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0a8d5-108">Here is a JSON representation of the resource</span></span>

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="0a8d5-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a8d5-109">Properties</span></span>

| <span data-ttu-id="0a8d5-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a8d5-110">Property</span></span>              | <span data-ttu-id="0a8d5-111">Typ</span><span class="sxs-lookup"><span data-stu-id="0a8d5-111">Type</span></span>          | <span data-ttu-id="0a8d5-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a8d5-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="0a8d5-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a8d5-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="0a8d5-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a8d5-114">DateTimeOffset</span></span>        | <span data-ttu-id="0a8d5-115">Das Datum und die Zeit, die die Ressource zuletzt vom Benutzer zugegriffen werden konnte.</span><span class="sxs-lookup"><span data-stu-id="0a8d5-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="0a8d5-116">Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="0a8d5-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0a8d5-117">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="0a8d5-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="0a8d5-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0a8d5-118">Read-only.</span></span>                      |
| <span data-ttu-id="0a8d5-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a8d5-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="0a8d5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a8d5-120">DateTimeOffset</span></span>        | <span data-ttu-id="0a8d5-121">Datum und Uhrzeit der letzten Änderung die Ressource durch den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="0a8d5-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="0a8d5-122">Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="0a8d5-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0a8d5-123">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="0a8d5-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="0a8d5-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0a8d5-124">Read-only.</span></span>       |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-usagedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
