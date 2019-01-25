---
title: Ressourcentyp historyItem
description: Stellt ein Verlaufselement für eine Aktivität in einer app. Die Benutzeraktivitäten darstellen ein einziges Ziel in der app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel. Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als Element Verlauf erfasst, das die Start- und Endzeit für diese Aktivität angibt. Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 640b2e777337182b95572ba086f1caf3459ef57e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514698"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="b532b-106">Ressourcentyp historyItem</span><span class="sxs-lookup"><span data-stu-id="b532b-106">historyItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b532b-107">Stellt ein Verlaufselement für eine [Aktivität](projectrome-activity.md) in einer app.</span><span class="sxs-lookup"><span data-stu-id="b532b-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="b532b-108">Die Benutzeraktivitäten darstellen ein einziges Ziel in der app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel.</span><span class="sxs-lookup"><span data-stu-id="b532b-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="b532b-109">Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als Element Verlauf erfasst, das die Start- und Endzeit für diese Aktivität angibt.</span><span class="sxs-lookup"><span data-stu-id="b532b-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="b532b-110">Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="b532b-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="b532b-111">Wenn eine app eine Sitzung erstellt, sollte ein **HistoryItem** -Objekt auf die **Aktivität** -Objekt entsprechend den Zeitraum eines Auftrags für Benutzer hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="b532b-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="b532b-112">Jedes Mal wird ein Benutzer mit einer Aktivität erneut aktiviert wird, eine neue **HistoryItem** Aktivität auf die Benutzer Engagements fällig hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b532b-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="b532b-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="b532b-113">Methods</span></span>

|<span data-ttu-id="b532b-114">Methode</span><span class="sxs-lookup"><span data-stu-id="b532b-114">Method</span></span> | <span data-ttu-id="b532b-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b532b-115">Return Type</span></span> | <span data-ttu-id="b532b-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b532b-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="b532b-117">Erstellen oder ersetzen historyItem</span><span class="sxs-lookup"><span data-stu-id="b532b-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="b532b-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="b532b-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="b532b-119">Erstellt oder eine vorhandene **HistoryItem** für diese Aktivität (Upsert) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="b532b-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="b532b-120">Die ID muss eine GUID sein.</span><span class="sxs-lookup"><span data-stu-id="b532b-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="b532b-121">Löschen einer historyItem</span><span class="sxs-lookup"><span data-stu-id="b532b-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="b532b-122">Kein Inhalt</span><span class="sxs-lookup"><span data-stu-id="b532b-122">No Content</span></span> | <span data-ttu-id="b532b-123">Löscht das angegebene **HistoryItem** für diese Aktivität.</span><span class="sxs-lookup"><span data-stu-id="b532b-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="b532b-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b532b-124">Properties</span></span>

|<span data-ttu-id="b532b-125">Name</span><span class="sxs-lookup"><span data-stu-id="b532b-125">Name</span></span> | <span data-ttu-id="b532b-126">Typ</span><span class="sxs-lookup"><span data-stu-id="b532b-126">Type</span></span> | <span data-ttu-id="b532b-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b532b-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="b532b-128">status</span><span class="sxs-lookup"><span data-stu-id="b532b-128">status</span></span> | <span data-ttu-id="b532b-129">EnumType</span><span class="sxs-lookup"><span data-stu-id="b532b-129">EnumType</span></span> | <span data-ttu-id="b532b-130">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b532b-130">Set by the server.</span></span> <span data-ttu-id="b532b-131">Einen Statuscode verwendet, um gültige Objekte identifizieren.</span><span class="sxs-lookup"><span data-stu-id="b532b-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="b532b-132">Werte: aktiv, aktualisiert, gelöscht, ignoriert.</span><span class="sxs-lookup"><span data-stu-id="b532b-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="b532b-133">userTimezone</span><span class="sxs-lookup"><span data-stu-id="b532b-133">userTimezone</span></span> | <span data-ttu-id="b532b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b532b-134">String</span></span> | <span data-ttu-id="b532b-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="b532b-135">Optional.</span></span> <span data-ttu-id="b532b-136">Die Zeitzone, in der das Gerät des Benutzers verwendet, um die Aktivität generieren zum Zeitpunkt der Erstellung Aktivität gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="b532b-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="b532b-137">Werte, die zur Unterstützung der plattformübergreifende Darstellung als Olson-IDs angegeben.</span><span class="sxs-lookup"><span data-stu-id="b532b-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="b532b-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b532b-138">createdDateTime</span></span> | <span data-ttu-id="b532b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b532b-139">DateTimeOffset</span></span> | <span data-ttu-id="b532b-140">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b532b-140">Set by the server.</span></span> <span data-ttu-id="b532b-141">DateTime in UTC, wenn das Objekt auf dem Server erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="b532b-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="b532b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b532b-142">lastModifiedDateTime</span></span> | <span data-ttu-id="b532b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b532b-143">DateTimeOffset</span></span> | <span data-ttu-id="b532b-144">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b532b-144">Set by the server.</span></span> <span data-ttu-id="b532b-145">DateTime in UTC, wenn das Objekt auf dem Server geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="b532b-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="b532b-146">id</span><span class="sxs-lookup"><span data-stu-id="b532b-146">id</span></span> | <span data-ttu-id="b532b-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b532b-147">String</span></span> | <span data-ttu-id="b532b-148">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b532b-148">Required.</span></span> <span data-ttu-id="b532b-149">Client-Set-GUID für das **HistoryItem** -Objekt.</span><span class="sxs-lookup"><span data-stu-id="b532b-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="b532b-150">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="b532b-150">startedDateTime</span></span> | <span data-ttu-id="b532b-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b532b-151">DateTimeOffset</span></span> | <span data-ttu-id="b532b-152">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b532b-152">Required.</span></span> <span data-ttu-id="b532b-153">UTC-DateTime beim **HistoryItem** (Aktivität Sitzung) gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="b532b-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="b532b-154">Erforderlich für die Versionsgeschichte der Zeitachse.</span><span class="sxs-lookup"><span data-stu-id="b532b-154">Required for timeline history.</span></span>|
|<span data-ttu-id="b532b-155">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="b532b-155">lastActiveDateTime</span></span> | <span data-ttu-id="b532b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b532b-156">DateTimeOffset</span></span> | <span data-ttu-id="b532b-157">Optional.</span><span class="sxs-lookup"><span data-stu-id="b532b-157">Optional.</span></span> <span data-ttu-id="b532b-158">UTC-DateTime beim letzten **HistoryItem** (Aktivität Sitzung) als aktiv oder fertig - bei null **HistoryItem** Status erkannt wurden, sollte laufend Besprechung sein.</span><span class="sxs-lookup"><span data-stu-id="b532b-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="b532b-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b532b-159">expirationDateTime</span></span> | <span data-ttu-id="b532b-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b532b-160">DateTimeOffset</span></span> | <span data-ttu-id="b532b-161">Optional.</span><span class="sxs-lookup"><span data-stu-id="b532b-161">Optional.</span></span> <span data-ttu-id="b532b-162">UTC-DateTime, wenn die **HistoryItem** harten Löschens durchläuft.</span><span class="sxs-lookup"><span data-stu-id="b532b-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="b532b-163">Kann vom Client festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b532b-163">Can be set by the client.</span></span>|
|<span data-ttu-id="b532b-164">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="b532b-164">activeDurationSeconds</span></span> | <span data-ttu-id="b532b-165">int</span><span class="sxs-lookup"><span data-stu-id="b532b-165">int</span></span> | <span data-ttu-id="b532b-166">Optional.</span><span class="sxs-lookup"><span data-stu-id="b532b-166">Optional.</span></span> <span data-ttu-id="b532b-167">Die Dauer des Engagements aktiver Benutzer.</span><span class="sxs-lookup"><span data-stu-id="b532b-167">The duration of active user engagement.</span></span> <span data-ttu-id="b532b-168">Wenn nicht angegeben ist, erfolgt die Berechnung von der **StartedDateTime** und **LastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="b532b-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b532b-169">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b532b-169">Relationships</span></span>

|<span data-ttu-id="b532b-170">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b532b-170">Relationship</span></span> | <span data-ttu-id="b532b-171">Typ</span><span class="sxs-lookup"><span data-stu-id="b532b-171">Type</span></span> | <span data-ttu-id="b532b-172">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b532b-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="b532b-173">activity</span><span class="sxs-lookup"><span data-stu-id="b532b-173">activity</span></span>| [<span data-ttu-id="b532b-174">Aktivität</span><span class="sxs-lookup"><span data-stu-id="b532b-174">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="b532b-175">Optional.</span><span class="sxs-lookup"><span data-stu-id="b532b-175">Optional.</span></span> <span data-ttu-id="b532b-176">NavigationProperty/Kapselung; Navigationseigenschaft der zugeordneten Aktivität.</span><span class="sxs-lookup"><span data-stu-id="b532b-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b532b-177">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b532b-177">JSON representation</span></span>

<span data-ttu-id="b532b-178">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b532b-178">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-historyitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
