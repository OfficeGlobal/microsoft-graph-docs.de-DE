---
title: Ressourcentyp historyItem
description: Stellt ein Verlaufselement für eine Aktivität in einer app. Die Benutzeraktivitäten darstellen ein einziges Ziel in der app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel. Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als Element Verlauf erfasst, das die Start- und Endzeit für diese Aktivität angibt. Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.
ms.openlocfilehash: 5687e592a65e162c105d97c90cd7a6f8f578d303
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065378"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="b3948-106">Ressourcentyp historyItem</span><span class="sxs-lookup"><span data-stu-id="b3948-106">historyItem resource type</span></span>

> <span data-ttu-id="b3948-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b3948-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3948-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3948-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3948-109">Stellt ein Verlaufselement für eine [Aktivität](projectrome-activity.md) in einer app.</span><span class="sxs-lookup"><span data-stu-id="b3948-109">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="b3948-110">Die Benutzeraktivitäten darstellen ein einziges Ziel in der app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel.</span><span class="sxs-lookup"><span data-stu-id="b3948-110">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="b3948-111">Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als Element Verlauf erfasst, das die Start- und Endzeit für diese Aktivität angibt.</span><span class="sxs-lookup"><span data-stu-id="b3948-111">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="b3948-112">Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="b3948-112">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="b3948-113">Wenn eine app eine Sitzung erstellt, sollte ein **HistoryItem** -Objekt auf die **Aktivität** -Objekt entsprechend den Zeitraum eines Auftrags für Benutzer hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="b3948-113">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="b3948-114">Jedes Mal wird ein Benutzer mit einer Aktivität erneut aktiviert wird, eine neue **HistoryItem** Aktivität auf die Benutzer Engagements fällig hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b3948-114">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="b3948-115">Methoden</span><span class="sxs-lookup"><span data-stu-id="b3948-115">Methods</span></span>

|<span data-ttu-id="b3948-116">Methode</span><span class="sxs-lookup"><span data-stu-id="b3948-116">Method</span></span> | <span data-ttu-id="b3948-117">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b3948-117">Return Type</span></span> | <span data-ttu-id="b3948-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3948-118">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="b3948-119">Erstellen oder ersetzen historyItem</span><span class="sxs-lookup"><span data-stu-id="b3948-119">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="b3948-120">historyItem</span><span class="sxs-lookup"><span data-stu-id="b3948-120">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="b3948-121">Erstellt oder eine vorhandene **HistoryItem** für diese Aktivität (Upsert) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="b3948-121">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="b3948-122">Die ID muss eine GUID sein.</span><span class="sxs-lookup"><span data-stu-id="b3948-122">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="b3948-123">Löschen einer historyItem</span><span class="sxs-lookup"><span data-stu-id="b3948-123">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="b3948-124">Kein Inhalt</span><span class="sxs-lookup"><span data-stu-id="b3948-124">No Content</span></span> | <span data-ttu-id="b3948-125">Löscht das angegebene **HistoryItem** für diese Aktivität.</span><span class="sxs-lookup"><span data-stu-id="b3948-125">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3948-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b3948-126">Properties</span></span>

|<span data-ttu-id="b3948-127">Name</span><span class="sxs-lookup"><span data-stu-id="b3948-127">Name</span></span> | <span data-ttu-id="b3948-128">Typ</span><span class="sxs-lookup"><span data-stu-id="b3948-128">Type</span></span> | <span data-ttu-id="b3948-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3948-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="b3948-130">status</span><span class="sxs-lookup"><span data-stu-id="b3948-130">status</span></span> | <span data-ttu-id="b3948-131">EnumType</span><span class="sxs-lookup"><span data-stu-id="b3948-131">EnumType</span></span> | <span data-ttu-id="b3948-132">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b3948-132">Set by the server.</span></span> <span data-ttu-id="b3948-133">Einen Statuscode verwendet, um gültige Objekte identifizieren.</span><span class="sxs-lookup"><span data-stu-id="b3948-133">A status code used to identify valid objects.</span></span> <span data-ttu-id="b3948-134">Werte: aktiv, aktualisiert, gelöscht, ignoriert.</span><span class="sxs-lookup"><span data-stu-id="b3948-134">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="b3948-135">userTimezone</span><span class="sxs-lookup"><span data-stu-id="b3948-135">userTimezone</span></span> | <span data-ttu-id="b3948-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3948-136">String</span></span> | <span data-ttu-id="b3948-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="b3948-137">Optional.</span></span> <span data-ttu-id="b3948-138">Die Zeitzone, in der das Gerät des Benutzers verwendet, um die Aktivität generieren zum Zeitpunkt der Erstellung Aktivität gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="b3948-138">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="b3948-139">Werte, die zur Unterstützung der plattformübergreifende Darstellung als Olson-IDs angegeben.</span><span class="sxs-lookup"><span data-stu-id="b3948-139">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="b3948-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3948-140">createdDateTime</span></span> | <span data-ttu-id="b3948-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3948-141">DateTimeOffset</span></span> | <span data-ttu-id="b3948-142">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b3948-142">Set by the server.</span></span> <span data-ttu-id="b3948-143">DateTime in UTC, wenn das Objekt auf dem Server erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="b3948-143">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="b3948-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3948-144">lastModifiedDateTime</span></span> | <span data-ttu-id="b3948-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3948-145">DateTimeOffset</span></span> | <span data-ttu-id="b3948-146">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b3948-146">Set by the server.</span></span> <span data-ttu-id="b3948-147">DateTime in UTC, wenn das Objekt auf dem Server geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="b3948-147">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="b3948-148">id</span><span class="sxs-lookup"><span data-stu-id="b3948-148">id</span></span> | <span data-ttu-id="b3948-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3948-149">String</span></span> | <span data-ttu-id="b3948-150">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b3948-150">Required.</span></span> <span data-ttu-id="b3948-151">Client-Set-GUID für das **HistoryItem** -Objekt.</span><span class="sxs-lookup"><span data-stu-id="b3948-151">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="b3948-152">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3948-152">startedDateTime</span></span> | <span data-ttu-id="b3948-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3948-153">DateTimeOffset</span></span> | <span data-ttu-id="b3948-154">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b3948-154">Required.</span></span> <span data-ttu-id="b3948-155">UTC-DateTime beim **HistoryItem** (Aktivität Sitzung) gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="b3948-155">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="b3948-156">Erforderlich für die Versionsgeschichte der Zeitachse.</span><span class="sxs-lookup"><span data-stu-id="b3948-156">Required for timeline history.</span></span>|
|<span data-ttu-id="b3948-157">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="b3948-157">lastActiveDateTime</span></span> | <span data-ttu-id="b3948-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3948-158">DateTimeOffset</span></span> | <span data-ttu-id="b3948-159">Optional.</span><span class="sxs-lookup"><span data-stu-id="b3948-159">Optional.</span></span> <span data-ttu-id="b3948-160">UTC-DateTime beim letzten **HistoryItem** (Aktivität Sitzung) als aktiv oder fertig - bei null **HistoryItem** Status erkannt wurden, sollte laufend Besprechung sein.</span><span class="sxs-lookup"><span data-stu-id="b3948-160">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="b3948-161">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b3948-161">expirationDateTime</span></span> | <span data-ttu-id="b3948-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3948-162">DateTimeOffset</span></span> | <span data-ttu-id="b3948-163">Optional.</span><span class="sxs-lookup"><span data-stu-id="b3948-163">Optional.</span></span> <span data-ttu-id="b3948-164">UTC-DateTime, wenn die **HistoryItem** harten Löschens durchläuft.</span><span class="sxs-lookup"><span data-stu-id="b3948-164">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="b3948-165">Kann vom Client festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b3948-165">Can be set by the client.</span></span>|
|<span data-ttu-id="b3948-166">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="b3948-166">activeDurationSeconds</span></span> | <span data-ttu-id="b3948-167">Int</span><span class="sxs-lookup"><span data-stu-id="b3948-167">int</span></span> | <span data-ttu-id="b3948-168">Optional.</span><span class="sxs-lookup"><span data-stu-id="b3948-168">Optional.</span></span> <span data-ttu-id="b3948-169">Die Dauer des Engagements aktiver Benutzer.</span><span class="sxs-lookup"><span data-stu-id="b3948-169">The duration of active user engagement.</span></span> <span data-ttu-id="b3948-170">Wenn nicht angegeben ist, erfolgt die Berechnung von der **StartedDateTime** und **LastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="b3948-170">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3948-171">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b3948-171">Relationships</span></span>

|<span data-ttu-id="b3948-172">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b3948-172">Relationship</span></span> | <span data-ttu-id="b3948-173">Typ</span><span class="sxs-lookup"><span data-stu-id="b3948-173">Type</span></span> | <span data-ttu-id="b3948-174">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3948-174">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="b3948-175">activity</span><span class="sxs-lookup"><span data-stu-id="b3948-175">activity</span></span>| [<span data-ttu-id="b3948-176">Aktivität</span><span class="sxs-lookup"><span data-stu-id="b3948-176">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="b3948-177">Optional.</span><span class="sxs-lookup"><span data-stu-id="b3948-177">Optional.</span></span> <span data-ttu-id="b3948-178">NavigationProperty/Kapselung; Navigationseigenschaft der zugeordneten Aktivität.</span><span class="sxs-lookup"><span data-stu-id="b3948-178">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3948-179">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b3948-179">JSON representation</span></span>

<span data-ttu-id="b3948-180">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b3948-180">Here is a JSON representation of the resource.</span></span>

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
