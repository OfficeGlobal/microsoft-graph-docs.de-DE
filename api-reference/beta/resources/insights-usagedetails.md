---
title: Ressourcentyp usageDetails
description: Komplexer Typ, die Eigenschaften des verwendeten Elemente enthält. Wenn die Ressource des letzten Zugriffs auf Informationen (Ansicht) und (bearbeitet) vom Benutzer geändert.
ms.openlocfilehash: c74b1436abcfa4993728371a79d2371a667a16d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058033"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="8f2cf-104">Ressourcentyp usageDetails</span><span class="sxs-lookup"><span data-stu-id="8f2cf-104">usageDetails resource type</span></span>

> <span data-ttu-id="8f2cf-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8f2cf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f2cf-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8f2cf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f2cf-107">Komplexer Typ, enthält die Eigenschaften von Elementen [verwendet](insights-used.md) .</span><span class="sxs-lookup"><span data-stu-id="8f2cf-107">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="8f2cf-108">Wenn die Ressource des letzten Zugriffs auf Informationen (Ansicht) und (bearbeitet) vom Benutzer geändert.</span><span class="sxs-lookup"><span data-stu-id="8f2cf-108">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f2cf-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8f2cf-109">JSON representation</span></span>

<span data-ttu-id="8f2cf-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f2cf-110">Here is a JSON representation of the resource</span></span>

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="8f2cf-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8f2cf-111">Properties</span></span>

| <span data-ttu-id="8f2cf-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f2cf-112">Property</span></span>              | <span data-ttu-id="8f2cf-113">Typ</span><span class="sxs-lookup"><span data-stu-id="8f2cf-113">Type</span></span>          | <span data-ttu-id="8f2cf-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f2cf-114">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="8f2cf-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f2cf-115">lastAccessedDateTime</span></span>                  | <span data-ttu-id="8f2cf-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f2cf-116">DateTimeOffset</span></span>        | <span data-ttu-id="8f2cf-117">Das Datum und die Zeit, die die Ressource zuletzt vom Benutzer zugegriffen werden konnte.</span><span class="sxs-lookup"><span data-stu-id="8f2cf-117">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="8f2cf-118">Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="8f2cf-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f2cf-119">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8f2cf-119">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8f2cf-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2cf-120">Read-only.</span></span>                      |
| <span data-ttu-id="8f2cf-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f2cf-121">lastModifiedDateTime</span></span>              | <span data-ttu-id="8f2cf-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f2cf-122">DateTimeOffset</span></span>        | <span data-ttu-id="8f2cf-123">Datum und Uhrzeit der letzten Änderung die Ressource durch den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="8f2cf-123">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="8f2cf-124">Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="8f2cf-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f2cf-125">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8f2cf-125">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8f2cf-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2cf-126">Read-only.</span></span>       |