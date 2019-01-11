---
title: recentNotebook-Ressourcentyp
description: Ein OneNote-Notizbuch, auf das kürzlich zugegriffen wurde. Ein **recentNotebook** ist vergleichbar mit einem Notizbuch, hat jedoch weniger Eigenschaften.
localization_priority: Normal
ms.openlocfilehash: 67c707043e5b6ca65cd72ddc323b5a484f0f2959
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889222"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="d2861-104">recentNotebook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d2861-104">recentNotebook resource type</span></span>

<span data-ttu-id="d2861-105">Ein OneNote-Notizbuch, auf das kürzlich zugegriffen wurde.</span><span class="sxs-lookup"><span data-stu-id="d2861-105">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="d2861-106">Ein **recentNotebook** ist vergleichbar mit einem [Notizbuch](notebook.md), hat jedoch weniger Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="d2861-106">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="d2861-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d2861-107">Properties</span></span>
| <span data-ttu-id="d2861-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2861-108">Property</span></span>     | <span data-ttu-id="d2861-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d2861-109">Type</span></span>   |<span data-ttu-id="d2861-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2861-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2861-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d2861-111">displayName</span></span>|<span data-ttu-id="d2861-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d2861-112">String</span></span>|<span data-ttu-id="d2861-113">Der Name des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="d2861-113">The name of the notebook.</span></span>|
|<span data-ttu-id="d2861-114">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="d2861-114">lastAccessedTime</span></span>|<span data-ttu-id="d2861-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2861-115">DateTimeOffset</span></span>|<span data-ttu-id="d2861-p103">Das Datum und die Uhrzeit der letzten Änderung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d2861-p103">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="d2861-120">Links</span><span class="sxs-lookup"><span data-stu-id="d2861-120">links</span></span>|[<span data-ttu-id="d2861-121">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="d2861-121">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="d2861-122">Links zum Öffnen des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="d2861-122">Links for opening the notebook.</span></span> <span data-ttu-id="d2861-123">Der Link `oneNoteClientURL` öffnet das Notizbuch im OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="d2861-123">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="d2861-124">Der Link `oneNoteWebURL` öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="d2861-124">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="d2861-125">sourceService</span><span class="sxs-lookup"><span data-stu-id="d2861-125">sourceService</span></span>|<span data-ttu-id="d2861-126">onenoteSourceService</span><span class="sxs-lookup"><span data-stu-id="d2861-126">onenoteSourceService</span></span>|<span data-ttu-id="d2861-127">Der Back-End-Speicher, in dem das Notizbuch gespeichert ist (entweder `OneDriveForBusiness` oder `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="d2861-127">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2861-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d2861-128">JSON representation</span></span>

<span data-ttu-id="d2861-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d2861-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}
```

## <a name="methods"></a><span data-ttu-id="d2861-130">Methoden</span><span class="sxs-lookup"><span data-stu-id="d2861-130">Methods</span></span>

| <span data-ttu-id="d2861-131">Methode</span><span class="sxs-lookup"><span data-stu-id="d2861-131">Method</span></span>           | <span data-ttu-id="d2861-132">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d2861-132">Return Type</span></span>    |<span data-ttu-id="d2861-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2861-133">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2861-134">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="d2861-134">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="d2861-135">Sammlung [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="d2861-135">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="d2861-136">Dient zum Abrufen einer Sammlung der zuletzt geöffneten Notizbücher des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d2861-136">Get a collection of the most recently accessed notebooks for the user.</span></span> |
