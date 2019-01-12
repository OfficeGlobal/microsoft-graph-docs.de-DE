---
title: Ressourcentyp historyItem
description: Stellt ein Verlaufselement für eine Aktivität in einer app. Die Benutzeraktivitäten darstellen ein einziges Ziel in der app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel. Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als Element Verlauf erfasst, das die Start- und Endzeit für diese Aktivität angibt. Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 168587aa54446aeee78107deaa9087c6bffb8586
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976954"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="3a536-106">Ressourcentyp historyItem</span><span class="sxs-lookup"><span data-stu-id="3a536-106">historyItem resource type</span></span>

> <span data-ttu-id="3a536-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3a536-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a536-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3a536-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a536-109">Stellt ein Verlaufselement für eine [Aktivität](projectrome-activity.md) in einer app.</span><span class="sxs-lookup"><span data-stu-id="3a536-109">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="3a536-110">Die Benutzeraktivitäten darstellen ein einziges Ziel in der app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel.</span><span class="sxs-lookup"><span data-stu-id="3a536-110">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="3a536-111">Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als Element Verlauf erfasst, das die Start- und Endzeit für diese Aktivität angibt.</span><span class="sxs-lookup"><span data-stu-id="3a536-111">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="3a536-112">Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="3a536-112">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="3a536-113">Wenn eine app eine Sitzung erstellt, sollte ein **HistoryItem** -Objekt auf die **Aktivität** -Objekt entsprechend den Zeitraum eines Auftrags für Benutzer hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="3a536-113">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="3a536-114">Jedes Mal wird ein Benutzer mit einer Aktivität erneut aktiviert wird, eine neue **HistoryItem** Aktivität auf die Benutzer Engagements fällig hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="3a536-114">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="3a536-115">Methoden</span><span class="sxs-lookup"><span data-stu-id="3a536-115">Methods</span></span>

|<span data-ttu-id="3a536-116">Methode</span><span class="sxs-lookup"><span data-stu-id="3a536-116">Method</span></span> | <span data-ttu-id="3a536-117">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3a536-117">Return Type</span></span> | <span data-ttu-id="3a536-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a536-118">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="3a536-119">Erstellen oder ersetzen historyItem</span><span class="sxs-lookup"><span data-stu-id="3a536-119">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="3a536-120">historyItem</span><span class="sxs-lookup"><span data-stu-id="3a536-120">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="3a536-121">Erstellt oder eine vorhandene **HistoryItem** für diese Aktivität (Upsert) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="3a536-121">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="3a536-122">Die ID muss eine GUID sein.</span><span class="sxs-lookup"><span data-stu-id="3a536-122">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="3a536-123">Löschen einer historyItem</span><span class="sxs-lookup"><span data-stu-id="3a536-123">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="3a536-124">Kein Inhalt</span><span class="sxs-lookup"><span data-stu-id="3a536-124">No Content</span></span> | <span data-ttu-id="3a536-125">Löscht das angegebene **HistoryItem** für diese Aktivität.</span><span class="sxs-lookup"><span data-stu-id="3a536-125">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="3a536-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3a536-126">Properties</span></span>

|<span data-ttu-id="3a536-127">Name</span><span class="sxs-lookup"><span data-stu-id="3a536-127">Name</span></span> | <span data-ttu-id="3a536-128">Typ</span><span class="sxs-lookup"><span data-stu-id="3a536-128">Type</span></span> | <span data-ttu-id="3a536-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a536-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="3a536-130">status</span><span class="sxs-lookup"><span data-stu-id="3a536-130">status</span></span> | <span data-ttu-id="3a536-131">EnumType</span><span class="sxs-lookup"><span data-stu-id="3a536-131">EnumType</span></span> | <span data-ttu-id="3a536-132">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="3a536-132">Set by the server.</span></span> <span data-ttu-id="3a536-133">Einen Statuscode verwendet, um gültige Objekte identifizieren.</span><span class="sxs-lookup"><span data-stu-id="3a536-133">A status code used to identify valid objects.</span></span> <span data-ttu-id="3a536-134">Werte: aktiv, aktualisiert, gelöscht, ignoriert.</span><span class="sxs-lookup"><span data-stu-id="3a536-134">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="3a536-135">userTimezone</span><span class="sxs-lookup"><span data-stu-id="3a536-135">userTimezone</span></span> | <span data-ttu-id="3a536-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a536-136">String</span></span> | <span data-ttu-id="3a536-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="3a536-137">Optional.</span></span> <span data-ttu-id="3a536-138">Die Zeitzone, in der das Gerät des Benutzers verwendet, um die Aktivität generieren zum Zeitpunkt der Erstellung Aktivität gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="3a536-138">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="3a536-139">Werte, die zur Unterstützung der plattformübergreifende Darstellung als Olson-IDs angegeben.</span><span class="sxs-lookup"><span data-stu-id="3a536-139">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="3a536-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a536-140">createdDateTime</span></span> | <span data-ttu-id="3a536-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a536-141">DateTimeOffset</span></span> | <span data-ttu-id="3a536-142">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="3a536-142">Set by the server.</span></span> <span data-ttu-id="3a536-143">DateTime in UTC, wenn das Objekt auf dem Server erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="3a536-143">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="3a536-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a536-144">lastModifiedDateTime</span></span> | <span data-ttu-id="3a536-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a536-145">DateTimeOffset</span></span> | <span data-ttu-id="3a536-146">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="3a536-146">Set by the server.</span></span> <span data-ttu-id="3a536-147">DateTime in UTC, wenn das Objekt auf dem Server geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="3a536-147">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="3a536-148">id</span><span class="sxs-lookup"><span data-stu-id="3a536-148">id</span></span> | <span data-ttu-id="3a536-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a536-149">String</span></span> | <span data-ttu-id="3a536-150">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a536-150">Required.</span></span> <span data-ttu-id="3a536-151">Client-Set-GUID für das **HistoryItem** -Objekt.</span><span class="sxs-lookup"><span data-stu-id="3a536-151">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="3a536-152">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a536-152">startedDateTime</span></span> | <span data-ttu-id="3a536-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a536-153">DateTimeOffset</span></span> | <span data-ttu-id="3a536-154">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="3a536-154">Required.</span></span> <span data-ttu-id="3a536-155">UTC-DateTime beim **HistoryItem** (Aktivität Sitzung) gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="3a536-155">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="3a536-156">Erforderlich für die Versionsgeschichte der Zeitachse.</span><span class="sxs-lookup"><span data-stu-id="3a536-156">Required for timeline history.</span></span>|
|<span data-ttu-id="3a536-157">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="3a536-157">lastActiveDateTime</span></span> | <span data-ttu-id="3a536-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a536-158">DateTimeOffset</span></span> | <span data-ttu-id="3a536-159">Optional.</span><span class="sxs-lookup"><span data-stu-id="3a536-159">Optional.</span></span> <span data-ttu-id="3a536-160">UTC-DateTime beim letzten **HistoryItem** (Aktivität Sitzung) als aktiv oder fertig - bei null **HistoryItem** Status erkannt wurden, sollte laufend Besprechung sein.</span><span class="sxs-lookup"><span data-stu-id="3a536-160">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="3a536-161">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3a536-161">expirationDateTime</span></span> | <span data-ttu-id="3a536-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a536-162">DateTimeOffset</span></span> | <span data-ttu-id="3a536-163">Optional.</span><span class="sxs-lookup"><span data-stu-id="3a536-163">Optional.</span></span> <span data-ttu-id="3a536-164">UTC-DateTime, wenn die **HistoryItem** harten Löschens durchläuft.</span><span class="sxs-lookup"><span data-stu-id="3a536-164">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="3a536-165">Kann vom Client festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="3a536-165">Can be set by the client.</span></span>|
|<span data-ttu-id="3a536-166">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="3a536-166">activeDurationSeconds</span></span> | <span data-ttu-id="3a536-167">int</span><span class="sxs-lookup"><span data-stu-id="3a536-167">int</span></span> | <span data-ttu-id="3a536-168">Optional.</span><span class="sxs-lookup"><span data-stu-id="3a536-168">Optional.</span></span> <span data-ttu-id="3a536-169">Die Dauer des Engagements aktiver Benutzer.</span><span class="sxs-lookup"><span data-stu-id="3a536-169">The duration of active user engagement.</span></span> <span data-ttu-id="3a536-170">Wenn nicht angegeben ist, erfolgt die Berechnung von der **StartedDateTime** und **LastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="3a536-170">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a536-171">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3a536-171">Relationships</span></span>

|<span data-ttu-id="3a536-172">Beziehung</span><span class="sxs-lookup"><span data-stu-id="3a536-172">Relationship</span></span> | <span data-ttu-id="3a536-173">Typ</span><span class="sxs-lookup"><span data-stu-id="3a536-173">Type</span></span> | <span data-ttu-id="3a536-174">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a536-174">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="3a536-175">activity</span><span class="sxs-lookup"><span data-stu-id="3a536-175">activity</span></span>| [<span data-ttu-id="3a536-176">Aktivität</span><span class="sxs-lookup"><span data-stu-id="3a536-176">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="3a536-177">Optional.</span><span class="sxs-lookup"><span data-stu-id="3a536-177">Optional.</span></span> <span data-ttu-id="3a536-178">NavigationProperty/Kapselung; Navigationseigenschaft der zugeordneten Aktivität.</span><span class="sxs-lookup"><span data-stu-id="3a536-178">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a536-179">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3a536-179">JSON representation</span></span>

<span data-ttu-id="3a536-180">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3a536-180">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "@odata.type": "microsoft.graph.historyItem"
}-->

```json
{
    "status": "String (EnumType)",
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
