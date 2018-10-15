# <a name="historyitem-resource-type"></a><span data-ttu-id="cd62a-101">Ressourcentyp historyItem</span><span class="sxs-lookup"><span data-stu-id="cd62a-101">historyItem resource type</span></span>

<span data-ttu-id="cd62a-102">Stellt ein Historienelement für eine [ Aktivität](projectrome_activity.md) in einer App dar.</span><span class="sxs-lookup"><span data-stu-id="cd62a-102">Represents a history item for an [activity](projectrome_activity.md) in an app.</span></span> <span data-ttu-id="cd62a-103">Benutzeraktivitäten stellen ein einziges Ziel in der App dar, beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Videospiel.</span><span class="sxs-lookup"><span data-stu-id="cd62a-103">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="cd62a-104">Wenn ein Benutzer diese Aktivität einbezieht, wird das Engagement als Element des Ereignisprotokolls erfasst, das die Start- und Endzeit für diese Aktivität angibt.</span><span class="sxs-lookup"><span data-stu-id="cd62a-104">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="cd62a-105">Wenn der Benutzer diese Aktivität im Laufe der Zeit erneut einbezieht, werden mehrere Elemente des Ereignisprotokolls als eine einzelne Benutzeraktivität aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="cd62a-105">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="cd62a-106">Wenn von einer Anwendung eine Sitzung erstellt wird, sollte ein **Historienelement** zum **Aktivität** -Objekt entsprechend dem Zeitraum eines Auftrags für Benutzer hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="cd62a-106">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="cd62a-107">Sobald ein Benutzer eine Aktivität wieder aufnimmt, wird der Aktivität ein neues **Historienelement** hinzugefügt, um das Benutzerengagement weiter ansteigen zu lassen.</span><span class="sxs-lookup"><span data-stu-id="cd62a-107">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="cd62a-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="cd62a-108">Methods</span></span>

|<span data-ttu-id="cd62a-109">Methode</span><span class="sxs-lookup"><span data-stu-id="cd62a-109">Method</span></span> | <span data-ttu-id="cd62a-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="cd62a-110">Return Type</span></span> | <span data-ttu-id="cd62a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd62a-111">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="cd62a-112">Erstellen oder Ersetzen eines Historienelements</span><span class="sxs-lookup"><span data-stu-id="cd62a-112">Create or replace historyItem</span></span>](../api/projectrome_put_historyitem.md) | <span data-ttu-id="cd62a-113">[historyItem](projectrome_historyitem.md)</span><span class="sxs-lookup"><span data-stu-id="cd62a-113">Added [historyItem](projectrome_historyitem.md)</span></span> | <span data-ttu-id="cd62a-114">Erstellt oder ersetzt ein vorhandenes **Historienelement** für diese Aktivität (Upsert).</span><span class="sxs-lookup"><span data-stu-id="cd62a-114">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="cd62a-115">Die ID muss eine GUID sein.</span><span class="sxs-lookup"><span data-stu-id="cd62a-115">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="cd62a-116">Löschen eines Historienelements</span><span class="sxs-lookup"><span data-stu-id="cd62a-116">Delete a historyItem</span></span>](../api/projectrome_delete_historyitem.md) | <span data-ttu-id="cd62a-117">Kein Inhalt</span><span class="sxs-lookup"><span data-stu-id="cd62a-117">204 No Content</span></span> | <span data-ttu-id="cd62a-118">Löscht das angegebene **Historienelement** für diese Aktivität.</span><span class="sxs-lookup"><span data-stu-id="cd62a-118">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd62a-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cd62a-119">Properties</span></span>

|<span data-ttu-id="cd62a-120">Name</span><span class="sxs-lookup"><span data-stu-id="cd62a-120">Name</span></span> | <span data-ttu-id="cd62a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="cd62a-121">Type</span></span> | <span data-ttu-id="cd62a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd62a-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="cd62a-123">status</span><span class="sxs-lookup"><span data-stu-id="cd62a-123">status</span></span> | <span data-ttu-id="cd62a-124">status</span><span class="sxs-lookup"><span data-stu-id="cd62a-124">status</span></span> | <span data-ttu-id="cd62a-125">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cd62a-125">Provided by the server.</span></span> <span data-ttu-id="cd62a-126">Ein Statuscode, der dazu verwendet wird, um gültige Objekte identifizieren.</span><span class="sxs-lookup"><span data-stu-id="cd62a-126">A status code used to identify valid objects.</span></span> <span data-ttu-id="cd62a-127">Werte: aktiv, aktualisiert, gelöscht, ignoriert.</span><span class="sxs-lookup"><span data-stu-id="cd62a-127">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="cd62a-128">Benutzer Zeitzone</span><span class="sxs-lookup"><span data-stu-id="cd62a-128">userTimezone</span></span> | <span data-ttu-id="cd62a-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd62a-129">String</span></span> | <span data-ttu-id="cd62a-130">Optional.</span><span class="sxs-lookup"><span data-stu-id="cd62a-130">Optional.</span></span> <span data-ttu-id="cd62a-131">Die Zeitzone, in der das Gerät des Benutzers zum Zeitpunkt der Erstellung der Aktivität verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="cd62a-131">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="cd62a-132">Werte, die zur Unterstützung der plattformübergreifenden Darstellung als Olson-IDs angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="cd62a-132">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="cd62a-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd62a-133">createdDateTime</span></span> | <span data-ttu-id="cd62a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd62a-134">DateTimeOffset</span></span> | <span data-ttu-id="cd62a-135">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cd62a-135">Provided by the server.</span></span> <span data-ttu-id="cd62a-136">DateTime in UTC, als das Objekt auf dem Server erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="cd62a-136">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="cd62a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd62a-137">lastModifiedDateTime</span></span> | <span data-ttu-id="cd62a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd62a-138">DateTimeOffset</span></span> | <span data-ttu-id="cd62a-139">Vom Server festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cd62a-139">Provided by the server.</span></span> <span data-ttu-id="cd62a-140">DateTime in UTC, als das Objekt auf dem Server geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="cd62a-140">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="cd62a-141">id</span><span class="sxs-lookup"><span data-stu-id="cd62a-141">id</span></span> | <span data-ttu-id="cd62a-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd62a-142">String</span></span> | <span data-ttu-id="cd62a-143">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd62a-143">Required.</span></span> <span data-ttu-id="cd62a-144">Vom Client festgelegte GUID für das **historyItem** -Objekt.</span><span class="sxs-lookup"><span data-stu-id="cd62a-144">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="cd62a-145">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd62a-145">startedDateTime</span></span> | <span data-ttu-id="cd62a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd62a-146">DateTimeOffset</span></span> | <span data-ttu-id="cd62a-147">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd62a-147">Required.</span></span> <span data-ttu-id="cd62a-148">UTC-DateTime zum Beginn des**historyItem** (Aktivitätssitzung).</span><span class="sxs-lookup"><span data-stu-id="cd62a-148">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="cd62a-149">Erforderlich für den Timeline-Verlauf.</span><span class="sxs-lookup"><span data-stu-id="cd62a-149">Required for timeline history.</span></span>|
|<span data-ttu-id="cd62a-150">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="cd62a-150">lastActiveDateTime</span></span> | <span data-ttu-id="cd62a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd62a-151">DateTimeOffset</span></span> | <span data-ttu-id="cd62a-152">Optional.</span><span class="sxs-lookup"><span data-stu-id="cd62a-152">Optional.</span></span> <span data-ttu-id="cd62a-153">UTC-DateTime beim letzten mal, als **Historienelement** (Aktivitätssitzung) als aktiv oder fertig verstanden wurden - bei null sollte der**Historienelement** Status laufend sein.</span><span class="sxs-lookup"><span data-stu-id="cd62a-153">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="cd62a-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cd62a-154">expirationDateTime</span></span> | <span data-ttu-id="cd62a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd62a-155">DateTimeOffset</span></span> | <span data-ttu-id="cd62a-156">Optional.</span><span class="sxs-lookup"><span data-stu-id="cd62a-156">Optional.</span></span> <span data-ttu-id="cd62a-157">UTC-DateTime, wenn das **Historienelement** endgültig gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="cd62a-157">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="cd62a-158">Kann vom Client festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="cd62a-158">Can be set by the client.</span></span>|
|<span data-ttu-id="cd62a-159">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="cd62a-159">activeDurationSeconds</span></span> | <span data-ttu-id="cd62a-160">int</span><span class="sxs-lookup"><span data-stu-id="cd62a-160">int</span></span> | <span data-ttu-id="cd62a-161">Optional.</span><span class="sxs-lookup"><span data-stu-id="cd62a-161">Optional.</span></span> <span data-ttu-id="cd62a-162">Die Dauer des Engagements aktiver Benutzer.</span><span class="sxs-lookup"><span data-stu-id="cd62a-162">The duration of active user engagement.</span></span> <span data-ttu-id="cd62a-163">Wenn nichts angegeben wurde, erfolgt die Berechnung durch **StartedDateTime** und **LastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="cd62a-163">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd62a-164">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cd62a-164">Relationships</span></span>

|<span data-ttu-id="cd62a-165">Beziehung</span><span class="sxs-lookup"><span data-stu-id="cd62a-165">Relationship</span></span> | <span data-ttu-id="cd62a-166">Typ</span><span class="sxs-lookup"><span data-stu-id="cd62a-166">Type</span></span> | <span data-ttu-id="cd62a-167">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd62a-167">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="cd62a-168">activity</span><span class="sxs-lookup"><span data-stu-id="cd62a-168">activity</span></span>| [<span data-ttu-id="cd62a-169">userActivity</span><span class="sxs-lookup"><span data-stu-id="cd62a-169">userActivity</span></span>](../resources/projectrome_activity.md) | <span data-ttu-id="cd62a-170">Optional.</span><span class="sxs-lookup"><span data-stu-id="cd62a-170">Optional.</span></span> <span data-ttu-id="cd62a-171">NavigationProperty/Kapselung; Navigationseigenschaft der zugeordneten Aktivität.</span><span class="sxs-lookup"><span data-stu-id="cd62a-171">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd62a-172">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cd62a-172">JSON representation</span></span>

<span data-ttu-id="cd62a-173">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cd62a-173">Here is a JSON representation of the resource.</span></span>

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
