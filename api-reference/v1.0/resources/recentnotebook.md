---
title: recentNotebook-Ressourcentyp
description: Ein OneNote-Notizbuch, auf das kürzlich zugegriffen wurde. Ein **recentNotebook** ist vergleichbar mit einem Notizbuch, hat jedoch weniger Eigenschaften.
ms.openlocfilehash: 7beeb23926210d5b8c2c364ceb81726c5a28becb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019811"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="60be6-104">recentNotebook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="60be6-104">recentNotebook resource type</span></span>

<span data-ttu-id="60be6-105">Ein OneNote-Notizbuch, auf das kürzlich zugegriffen wurde.</span><span class="sxs-lookup"><span data-stu-id="60be6-105">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="60be6-106">Ein **recentNotebook** ist vergleichbar mit einem [Notizbuch](notebook.md), hat jedoch weniger Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="60be6-106">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="60be6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="60be6-107">Properties</span></span>
| <span data-ttu-id="60be6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60be6-108">Property</span></span>     | <span data-ttu-id="60be6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="60be6-109">Type</span></span>   |<span data-ttu-id="60be6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60be6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60be6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="60be6-111">displayName</span></span>|<span data-ttu-id="60be6-112">String</span><span class="sxs-lookup"><span data-stu-id="60be6-112">String</span></span>|<span data-ttu-id="60be6-113">Der Name des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="60be6-113">The name of the notebook.</span></span>|
|<span data-ttu-id="60be6-114">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="60be6-114">lastAccessedTime</span></span>|<span data-ttu-id="60be6-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60be6-115">DateTimeOffset</span></span>|<span data-ttu-id="60be6-p103">Das Datum und die Uhrzeit der letzten Änderung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="60be6-p103">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="60be6-120">Links</span><span class="sxs-lookup"><span data-stu-id="60be6-120">links</span></span>|[<span data-ttu-id="60be6-121">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="60be6-121">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="60be6-122">Links zum Öffnen des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="60be6-122">Links for opening the notebook.</span></span> <span data-ttu-id="60be6-123">Der Link `oneNoteClientURL` öffnet das Notizbuch im OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="60be6-123">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="60be6-124">Der Link `oneNoteWebURL` öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="60be6-124">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="60be6-125">sourceService</span><span class="sxs-lookup"><span data-stu-id="60be6-125">sourceService</span></span>|<span data-ttu-id="60be6-126">onenoteSourceService</span><span class="sxs-lookup"><span data-stu-id="60be6-126">onenoteSourceService</span></span>|<span data-ttu-id="60be6-127">Der Back-End-Speicher, in dem das Notizbuch gespeichert ist (entweder `OneDriveForBusiness` oder `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="60be6-127">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60be6-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="60be6-128">JSON representation</span></span>

<span data-ttu-id="60be6-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="60be6-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="60be6-130">Methoden</span><span class="sxs-lookup"><span data-stu-id="60be6-130">Methods</span></span>

| <span data-ttu-id="60be6-131">Methode</span><span class="sxs-lookup"><span data-stu-id="60be6-131">Method</span></span>           | <span data-ttu-id="60be6-132">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="60be6-132">Return Type</span></span>    |<span data-ttu-id="60be6-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60be6-133">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="60be6-134">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="60be6-134">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="60be6-135">Sammlung [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="60be6-135">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="60be6-136">Dient zum Abrufen einer Sammlung der zuletzt geöffneten Notizbücher des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="60be6-136">Get a collection of the most recently accessed notebooks for the user.</span></span> |
