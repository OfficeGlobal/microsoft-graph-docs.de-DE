---
title: Ressourcentyp usageDetails
description: Komplexer Typ, die Eigenschaften des verwendeten Elemente enthält. Wenn die Ressource des letzten Zugriffs auf Informationen (Ansicht) und (bearbeitet) vom Benutzer geändert.
author: simonhult
ms.openlocfilehash: ef5efcfce439e9d08784637cb02657d7cd37adf7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349350"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="c7567-104">Ressourcentyp usageDetails</span><span class="sxs-lookup"><span data-stu-id="c7567-104">usageDetails resource type</span></span>

> <span data-ttu-id="c7567-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c7567-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7567-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7567-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7567-107">Komplexer Typ, enthält die Eigenschaften von Elementen [verwendet](insights-used.md) .</span><span class="sxs-lookup"><span data-stu-id="c7567-107">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="c7567-108">Wenn die Ressource des letzten Zugriffs auf Informationen (Ansicht) und (bearbeitet) vom Benutzer geändert.</span><span class="sxs-lookup"><span data-stu-id="c7567-108">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7567-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c7567-109">JSON representation</span></span>

<span data-ttu-id="c7567-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c7567-110">Here is a JSON representation of the resource</span></span>

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="c7567-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7567-111">Properties</span></span>

| <span data-ttu-id="c7567-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7567-112">Property</span></span>              | <span data-ttu-id="c7567-113">Typ</span><span class="sxs-lookup"><span data-stu-id="c7567-113">Type</span></span>          | <span data-ttu-id="c7567-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7567-114">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="c7567-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7567-115">lastAccessedDateTime</span></span>                  | <span data-ttu-id="c7567-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7567-116">DateTimeOffset</span></span>        | <span data-ttu-id="c7567-117">Das Datum und die Zeit, die die Ressource zuletzt vom Benutzer zugegriffen werden konnte.</span><span class="sxs-lookup"><span data-stu-id="c7567-117">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="c7567-118">Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="c7567-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c7567-119">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c7567-119">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="c7567-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c7567-120">Read-only.</span></span>                      |
| <span data-ttu-id="c7567-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7567-121">lastModifiedDateTime</span></span>              | <span data-ttu-id="c7567-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7567-122">DateTimeOffset</span></span>        | <span data-ttu-id="c7567-123">Datum und Uhrzeit der letzten Änderung die Ressource durch den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="c7567-123">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="c7567-124">Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="c7567-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c7567-125">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c7567-125">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="c7567-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c7567-126">Read-only.</span></span>       |