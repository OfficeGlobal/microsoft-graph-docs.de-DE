---
title: recentNotebook-Ressourcentyp
description: Ein OneNote-Notizbuch, auf das kürzlich zugegriffen wurde. Ein **recentNotebook** ist vergleichbar mit einem Notizbuch, hat jedoch weniger Eigenschaften.
ms.openlocfilehash: c3b717fcebdc229864aefe13c6452ce5eb95fc53
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061884"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="65e35-104">recentNotebook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="65e35-104">recentNotebook resource type</span></span>

> <span data-ttu-id="65e35-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="65e35-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65e35-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65e35-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65e35-107">Ein OneNote-Notizbuch, auf das kürzlich zugegriffen wurde.</span><span class="sxs-lookup"><span data-stu-id="65e35-107">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="65e35-108">Ein **recentNotebook** ist vergleichbar mit einem [Notizbuch](notebook.md), hat jedoch weniger Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="65e35-108">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="65e35-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="65e35-109">Properties</span></span>
| <span data-ttu-id="65e35-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65e35-110">Property</span></span>     | <span data-ttu-id="65e35-111">Typ</span><span class="sxs-lookup"><span data-stu-id="65e35-111">Type</span></span>   |<span data-ttu-id="65e35-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65e35-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65e35-113">name</span><span class="sxs-lookup"><span data-stu-id="65e35-113">name</span></span>|<span data-ttu-id="65e35-114">String</span><span class="sxs-lookup"><span data-stu-id="65e35-114">String</span></span>|<span data-ttu-id="65e35-115">Der Name des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="65e35-115">The name of the notebook.</span></span>|
|<span data-ttu-id="65e35-116">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="65e35-116">lastAccessedTime</span></span>|<span data-ttu-id="65e35-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65e35-117">DateTimeOffset</span></span>|<span data-ttu-id="65e35-p104">Das Datum und die Uhrzeit der letzten Änderung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="65e35-p104">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="65e35-122">Links</span><span class="sxs-lookup"><span data-stu-id="65e35-122">links</span></span>|[<span data-ttu-id="65e35-123">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="65e35-123">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="65e35-124">Links zum Öffnen des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="65e35-124">Links for opening the notebook.</span></span> <span data-ttu-id="65e35-125">Der Link `oneNoteClientURL` öffnet das Notizbuch im OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="65e35-125">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="65e35-126">Der Link `oneNoteWebURL` öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="65e35-126">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="65e35-127">sourceService</span><span class="sxs-lookup"><span data-stu-id="65e35-127">sourceService</span></span>|<span data-ttu-id="65e35-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65e35-128">String</span></span>|<span data-ttu-id="65e35-129">Der Back-End-Speicher, in dem das Notizbuch gespeichert ist (entweder `OneDriveForBusiness` oder `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="65e35-129">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65e35-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="65e35-130">JSON representation</span></span>

<span data-ttu-id="65e35-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="65e35-131">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="65e35-132">Methoden</span><span class="sxs-lookup"><span data-stu-id="65e35-132">Methods</span></span>

| <span data-ttu-id="65e35-133">Methode</span><span class="sxs-lookup"><span data-stu-id="65e35-133">Method</span></span>           | <span data-ttu-id="65e35-134">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="65e35-134">Return Type</span></span>    |<span data-ttu-id="65e35-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65e35-135">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65e35-136">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="65e35-136">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="65e35-137">Sammlung [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="65e35-137">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="65e35-138">Dient zum Abrufen einer Sammlung der zuletzt geöffneten Notizbücher des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="65e35-138">Get a collection of the most recently accessed notebooks for the user.</span></span> |
