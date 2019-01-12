---
title: Ressourcentyp historyItem
description: Stellt ein Verlaufselement für eine Aktivität in einer app. Die Benutzeraktivitäten darstellen ein einziges Ziel in der app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel. Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als Element Verlauf erfasst, das die Start- und Endzeit für diese Aktivität angibt. Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 029c17e09348977752f3ce5632740b2bdac64e46
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977437"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="a5509-106">Ressourcentyp historyItem</span><span class="sxs-lookup"><span data-stu-id="a5509-106">historyItem resource type</span></span>

<span data-ttu-id="a5509-107">Stellt ein Verlaufselement für eine [Aktivität](projectrome-activity.md) in einer app.</span><span class="sxs-lookup"><span data-stu-id="a5509-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="a5509-108">Die Benutzeraktivitäten darstellen ein einziges Ziel in der app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel.</span><span class="sxs-lookup"><span data-stu-id="a5509-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="a5509-109">Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als Element Verlauf erfasst, das die Start- und Endzeit für diese Aktivität angibt.</span><span class="sxs-lookup"><span data-stu-id="a5509-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="a5509-110">Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="a5509-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="a5509-111">Wenn eine app eine Sitzung erstellt, sollte ein **HistoryItem** -Objekt auf die **Aktivität** -Objekt entsprechend den Zeitraum eines Auftrags für Benutzer hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="a5509-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="a5509-112">Jedes Mal wird ein Benutzer mit einer Aktivität erneut aktiviert wird, eine neue **HistoryItem** Aktivität auf die Benutzer Engagements fällig hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="a5509-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="a5509-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="a5509-113">Methods</span></span>

|<span data-ttu-id="a5509-114">Methode</span><span class="sxs-lookup"><span data-stu-id="a5509-114">Method</span></span> | <span data-ttu-id="a5509-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a5509-115">Return Type</span></span> | <span data-ttu-id="a5509-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5509-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="a5509-117">Erstellen oder ersetzen historyItem</span><span class="sxs-lookup"><span data-stu-id="a5509-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="a5509-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="a5509-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="a5509-119">Erstellt oder eine vorhandene **HistoryItem** für diese Aktivität (Upsert) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="a5509-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="a5509-120">Die ID muss eine GUID sein.</span><span class="sxs-lookup"><span data-stu-id="a5509-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="a5509-121">Löschen einer historyItem</span><span class="sxs-lookup"><span data-stu-id="a5509-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="a5509-122">Kein Inhalt</span><span class="sxs-lookup"><span data-stu-id="a5509-122">No Content</span></span> | <span data-ttu-id="a5509-123">Löscht das angegebene **HistoryItem** für diese Aktivität.</span><span class="sxs-lookup"><span data-stu-id="a5509-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="a5509-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a5509-124">Properties</span></span>

|<span data-ttu-id="a5509-125">Name</span><span class="sxs-lookup"><span data-stu-id="a5509-125">Name</span></span> | <span data-ttu-id="a5509-126">Typ</span><span class="sxs-lookup"><span data-stu-id="a5509-126">Type</span></span> | <span data-ttu-id="a5509-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5509-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="a5509-128">status</span><span class="sxs-lookup"><span data-stu-id="a5509-128">status</span></span> | <span data-ttu-id="a5509-129">status</span><span class="sxs-lookup"><span data-stu-id="a5509-129">status</span></span> | <span data-ttu-id="a5509-130">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="a5509-130">Set by the server.</span></span> <span data-ttu-id="a5509-131">Einen Statuscode verwendet, um gültige Objekte identifizieren.</span><span class="sxs-lookup"><span data-stu-id="a5509-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="a5509-132">Werte: aktiv, aktualisiert, gelöscht, ignoriert.</span><span class="sxs-lookup"><span data-stu-id="a5509-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="a5509-133">userTimezone</span><span class="sxs-lookup"><span data-stu-id="a5509-133">userTimezone</span></span> | <span data-ttu-id="a5509-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5509-134">String</span></span> | <span data-ttu-id="a5509-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="a5509-135">Optional.</span></span> <span data-ttu-id="a5509-136">Die Zeitzone, in der das Gerät des Benutzers verwendet, um die Aktivität generieren zum Zeitpunkt der Erstellung Aktivität gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="a5509-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="a5509-137">Werte, die zur Unterstützung der plattformübergreifende Darstellung als Olson-IDs angegeben.</span><span class="sxs-lookup"><span data-stu-id="a5509-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="a5509-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5509-138">createdDateTime</span></span> | <span data-ttu-id="a5509-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5509-139">DateTimeOffset</span></span> | <span data-ttu-id="a5509-140">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="a5509-140">Set by the server.</span></span> <span data-ttu-id="a5509-141">DateTime in UTC, wenn das Objekt auf dem Server erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="a5509-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="a5509-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5509-142">lastModifiedDateTime</span></span> | <span data-ttu-id="a5509-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5509-143">DateTimeOffset</span></span> | <span data-ttu-id="a5509-144">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="a5509-144">Set by the server.</span></span> <span data-ttu-id="a5509-145">DateTime in UTC, wenn das Objekt auf dem Server geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="a5509-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="a5509-146">id</span><span class="sxs-lookup"><span data-stu-id="a5509-146">id</span></span> | <span data-ttu-id="a5509-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5509-147">String</span></span> | <span data-ttu-id="a5509-148">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a5509-148">Required.</span></span> <span data-ttu-id="a5509-149">Client-Set-GUID für das **HistoryItem** -Objekt.</span><span class="sxs-lookup"><span data-stu-id="a5509-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="a5509-150">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5509-150">startedDateTime</span></span> | <span data-ttu-id="a5509-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5509-151">DateTimeOffset</span></span> | <span data-ttu-id="a5509-152">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="a5509-152">Required.</span></span> <span data-ttu-id="a5509-153">UTC-DateTime beim **HistoryItem** (Aktivität Sitzung) gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="a5509-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="a5509-154">Erforderlich für die Versionsgeschichte der Zeitachse.</span><span class="sxs-lookup"><span data-stu-id="a5509-154">Required for timeline history.</span></span>|
|<span data-ttu-id="a5509-155">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="a5509-155">lastActiveDateTime</span></span> | <span data-ttu-id="a5509-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5509-156">DateTimeOffset</span></span> | <span data-ttu-id="a5509-157">Optional.</span><span class="sxs-lookup"><span data-stu-id="a5509-157">Optional.</span></span> <span data-ttu-id="a5509-158">UTC-DateTime beim letzten **HistoryItem** (Aktivität Sitzung) als aktiv oder fertig - bei null **HistoryItem** Status erkannt wurden, sollte laufend Besprechung sein.</span><span class="sxs-lookup"><span data-stu-id="a5509-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="a5509-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a5509-159">expirationDateTime</span></span> | <span data-ttu-id="a5509-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5509-160">DateTimeOffset</span></span> | <span data-ttu-id="a5509-161">Optional.</span><span class="sxs-lookup"><span data-stu-id="a5509-161">Optional.</span></span> <span data-ttu-id="a5509-162">UTC-DateTime, wenn die **HistoryItem** harten Löschens durchläuft.</span><span class="sxs-lookup"><span data-stu-id="a5509-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="a5509-163">Kann vom Client festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="a5509-163">Can be set by the client.</span></span>|
|<span data-ttu-id="a5509-164">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="a5509-164">activeDurationSeconds</span></span> | <span data-ttu-id="a5509-165">int</span><span class="sxs-lookup"><span data-stu-id="a5509-165">int</span></span> | <span data-ttu-id="a5509-166">Optional.</span><span class="sxs-lookup"><span data-stu-id="a5509-166">Optional.</span></span> <span data-ttu-id="a5509-167">Die Dauer des Engagements aktiver Benutzer.</span><span class="sxs-lookup"><span data-stu-id="a5509-167">The duration of active user engagement.</span></span> <span data-ttu-id="a5509-168">Wenn nicht angegeben ist, erfolgt die Berechnung von der **StartedDateTime** und **LastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="a5509-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5509-169">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a5509-169">Relationships</span></span>

|<span data-ttu-id="a5509-170">Beziehung</span><span class="sxs-lookup"><span data-stu-id="a5509-170">Relationship</span></span> | <span data-ttu-id="a5509-171">Typ</span><span class="sxs-lookup"><span data-stu-id="a5509-171">Type</span></span> | <span data-ttu-id="a5509-172">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5509-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="a5509-173">activity</span><span class="sxs-lookup"><span data-stu-id="a5509-173">activity</span></span>| [<span data-ttu-id="a5509-174">userActivity</span><span class="sxs-lookup"><span data-stu-id="a5509-174">userActivity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="a5509-175">Optional.</span><span class="sxs-lookup"><span data-stu-id="a5509-175">Optional.</span></span> <span data-ttu-id="a5509-176">NavigationProperty/Kapselung; Navigationseigenschaft der zugeordneten Aktivität.</span><span class="sxs-lookup"><span data-stu-id="a5509-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5509-177">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a5509-177">JSON representation</span></span>

<span data-ttu-id="a5509-178">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a5509-178">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
