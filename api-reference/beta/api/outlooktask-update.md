---
title: Outlooktask aktualisieren
description: Schreibbare Eigenschaften einer Outlook-Aufgabe zu ändern.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1908d9b918b13f87b1d5ab61dab912577f06da64
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526886"
---
# <a name="update-outlooktask"></a><span data-ttu-id="13343-103">Outlooktask aktualisieren</span><span class="sxs-lookup"><span data-stu-id="13343-103">Update outlooktask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13343-104">Schreibbare Eigenschaften einer Outlook-Aufgabe zu ändern.</span><span class="sxs-lookup"><span data-stu-id="13343-104">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="13343-105">Die Eigenschaft **CompletedDateTime** kann mit der Aktion **Complete** oder explizit mit einer PATCH-Operation gesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="13343-105">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="13343-106">Wenn Sie PATCH für die Einstellung von **CompletedDateTime** verwenden, stellen Sie sicher, dass Sie **Status** ebenfalls auf `completed` einstellen.</span><span class="sxs-lookup"><span data-stu-id="13343-106">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="13343-107">Standardmäßig wird dieses Vorgangs (und die POST, GET und [Abschließen von](../api/outlooktask-complete.md) Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13343-107">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="13343-108">Sie können mit dem `Prefer: outlook.timezone`-Header alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darstellen.</span><span class="sxs-lookup"><span data-stu-id="13343-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="13343-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="13343-109">Permissions</span></span>

<span data-ttu-id="13343-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13343-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13343-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13343-112">Permission type</span></span>      | <span data-ttu-id="13343-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13343-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13343-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13343-114">Delegated (work or school account)</span></span> | <span data-ttu-id="13343-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13343-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="13343-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13343-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13343-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13343-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="13343-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13343-118">Application</span></span> | <span data-ttu-id="13343-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13343-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13343-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13343-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="13343-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13343-121">Request headers</span></span>

| <span data-ttu-id="13343-122">Name</span><span class="sxs-lookup"><span data-stu-id="13343-122">Name</span></span>       | <span data-ttu-id="13343-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13343-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="13343-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="13343-124">Authorization</span></span>  | <span data-ttu-id="13343-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="13343-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13343-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="13343-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="13343-128">Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="13343-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="13343-129">Optional.</span><span class="sxs-lookup"><span data-stu-id="13343-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13343-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13343-130">Request body</span></span>

<span data-ttu-id="13343-p106">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="13343-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="13343-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13343-134">Property</span></span> | <span data-ttu-id="13343-135">Typ</span><span class="sxs-lookup"><span data-stu-id="13343-135">Type</span></span> | <span data-ttu-id="13343-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13343-136">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="13343-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="13343-137">assignedTo</span></span>|<span data-ttu-id="13343-138">String</span><span class="sxs-lookup"><span data-stu-id="13343-138">String</span></span>|<span data-ttu-id="13343-139">Der Name der Person, die die Aufgabe zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="13343-139">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="13343-140">body</span><span class="sxs-lookup"><span data-stu-id="13343-140">body</span></span>|[<span data-ttu-id="13343-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="13343-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="13343-142">Der Hauptteil der Aufgabe, die in der Regel Informationen zum Vorgang enthält.</span><span class="sxs-lookup"><span data-stu-id="13343-142">The task body that typically contains information about the task.</span></span> <span data-ttu-id="13343-143">Beachten Sie, dass nur HTML-Typ unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="13343-143">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="13343-144">categories</span><span class="sxs-lookup"><span data-stu-id="13343-144">categories</span></span>|<span data-ttu-id="13343-145">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="13343-145">String collection</span></span>|<span data-ttu-id="13343-146">Die Kategorien, die dem Vorgang zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="13343-146">The categories associated with the task.</span></span>|
|<span data-ttu-id="13343-147">changeKey</span><span class="sxs-lookup"><span data-stu-id="13343-147">changeKey</span></span>|<span data-ttu-id="13343-148">String</span><span class="sxs-lookup"><span data-stu-id="13343-148">String</span></span>|<span data-ttu-id="13343-149">Die Version des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="13343-149">The version of the task.</span></span>|
|<span data-ttu-id="13343-150">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="13343-150">completedDateTime</span></span>|[<span data-ttu-id="13343-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="13343-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="13343-152">Das Datum in der angegebenen Zeitzone, dass der Vorgang abgeschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="13343-152">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="13343-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13343-153">createdDateTime</span></span>|<span data-ttu-id="13343-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13343-154">DateTimeOffset</span></span>|<span data-ttu-id="13343-155">Datum und Uhrzeit der Erstellung die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="13343-155">The date and time when the task was created.</span></span> <span data-ttu-id="13343-156">Standardmäßig ist es in UTC.</span><span class="sxs-lookup"><span data-stu-id="13343-156">By default, it is in UTC.</span></span> <span data-ttu-id="13343-157">Sie können eine benutzerdefinierte Zeitzone in der Kopfzeile der Anforderung bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="13343-157">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="13343-158">Wert der Eigenschaft verwendet die ISO 8601-Format.</span><span class="sxs-lookup"><span data-stu-id="13343-158">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="13343-159">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="13343-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="13343-160">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="13343-160">dueDateTime</span></span>|[<span data-ttu-id="13343-161">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="13343-161">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="13343-162">Das Datum in der angegebenen Zeitzone, die die Aufgabe fertig gestellt werden.</span><span class="sxs-lookup"><span data-stu-id="13343-162">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="13343-163">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="13343-163">hasAttachments</span></span>|<span data-ttu-id="13343-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13343-164">Boolean</span></span>|<span data-ttu-id="13343-165">Legen Sie auf true zurück, wenn der Vorgang Anlagen hat.</span><span class="sxs-lookup"><span data-stu-id="13343-165">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="13343-166">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="13343-166">importance</span></span>|<span data-ttu-id="13343-167">string</span><span class="sxs-lookup"><span data-stu-id="13343-167">string</span></span>|<span data-ttu-id="13343-168">Die Wichtigkeit des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="13343-168">The importance of the event.</span></span> <span data-ttu-id="13343-169">Mögliche Werte sind: `low`, `normal` und `high`.</span><span class="sxs-lookup"><span data-stu-id="13343-169">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="13343-170">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="13343-170">isReminderOn</span></span>|<span data-ttu-id="13343-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="13343-171">Boolean</span></span>|<span data-ttu-id="13343-172">Legen Sie auf true zurück, wenn eine Warnung festgelegt ist, um die Benutzer über die Aufgabe zu erinnern.</span><span class="sxs-lookup"><span data-stu-id="13343-172">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="13343-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13343-173">lastModifiedDateTime</span></span>|<span data-ttu-id="13343-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13343-174">DateTimeOffset</span></span>|<span data-ttu-id="13343-175">Datum und Uhrzeit der letzten die Aufgabe Änderung.</span><span class="sxs-lookup"><span data-stu-id="13343-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="13343-176">Standardmäßig ist es in UTC.</span><span class="sxs-lookup"><span data-stu-id="13343-176">By default, it is in UTC.</span></span> <span data-ttu-id="13343-177">Sie können eine benutzerdefinierte Zeitzone in der Kopfzeile der Anforderung bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="13343-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="13343-178">Wert der Eigenschaft um ISO 8601-Format verwendet und ist immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="13343-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="13343-179">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="13343-179">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="13343-180">owner</span><span class="sxs-lookup"><span data-stu-id="13343-180">owner</span></span>|<span data-ttu-id="13343-181">String</span><span class="sxs-lookup"><span data-stu-id="13343-181">String</span></span>|<span data-ttu-id="13343-182">Der Name der Person, die die Aufgabe erstellt.</span><span class="sxs-lookup"><span data-stu-id="13343-182">The name of the person who created the task.</span></span>|
|<span data-ttu-id="13343-183">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="13343-183">parentFolderId</span></span>|<span data-ttu-id="13343-184">String</span><span class="sxs-lookup"><span data-stu-id="13343-184">String</span></span>|<span data-ttu-id="13343-185">Der eindeutige Bezeichner für die Aufgabe übergeordneten Ordner.</span><span class="sxs-lookup"><span data-stu-id="13343-185">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="13343-186">recurrence</span><span class="sxs-lookup"><span data-stu-id="13343-186">recurrence</span></span>|[<span data-ttu-id="13343-187">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="13343-187">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="13343-188">Das Serienmuster für den Vorgang.</span><span class="sxs-lookup"><span data-stu-id="13343-188">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="13343-189">ReminderDateTime</span><span class="sxs-lookup"><span data-stu-id="13343-189">reminderDateTime</span></span>|[<span data-ttu-id="13343-190">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="13343-190">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="13343-191">Datum und Zeit für eine Erinnerung des Vorgangs erfolgt.</span><span class="sxs-lookup"><span data-stu-id="13343-191">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="13343-192">sensitivity</span><span class="sxs-lookup"><span data-stu-id="13343-192">sensitivity</span></span>|<span data-ttu-id="13343-193">string</span><span class="sxs-lookup"><span data-stu-id="13343-193">string</span></span>|<span data-ttu-id="13343-194">Gibt die Ebene des Datenschutzes für den Vorgang an.</span><span class="sxs-lookup"><span data-stu-id="13343-194">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="13343-195">Mögliche Werte: sind `normal`, `personal`, `private` und `confidential`.</span><span class="sxs-lookup"><span data-stu-id="13343-195">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="13343-196">startDateTime</span><span class="sxs-lookup"><span data-stu-id="13343-196">startDateTime</span></span>|[<span data-ttu-id="13343-197">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="13343-197">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="13343-198">Das Datum in der angegebenen Zeitzone, wenn der Vorgang zu beginnen.</span><span class="sxs-lookup"><span data-stu-id="13343-198">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="13343-199">status</span><span class="sxs-lookup"><span data-stu-id="13343-199">status</span></span>|<span data-ttu-id="13343-200">string</span><span class="sxs-lookup"><span data-stu-id="13343-200">string</span></span>|<span data-ttu-id="13343-201">Gibt das Bundesland oder den Fortschritt des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="13343-201">Indicates the state or progress of the task.</span></span> <span data-ttu-id="13343-202">Mögliche Werte sind: `notStarted`, `inProgress`, `completed`, `waitingOnOthers` und `deferred`.</span><span class="sxs-lookup"><span data-stu-id="13343-202">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="13343-203">subject</span><span class="sxs-lookup"><span data-stu-id="13343-203">subject</span></span>|<span data-ttu-id="13343-204">String</span><span class="sxs-lookup"><span data-stu-id="13343-204">String</span></span>|<span data-ttu-id="13343-205">Eine kurze Beschreibung oder Titel des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="13343-205">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="13343-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="13343-206">Response</span></span>

<span data-ttu-id="13343-207">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [OutlookTask](../resources/outlooktask.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="13343-207">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13343-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13343-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="13343-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13343-209">Request</span></span>

<span data-ttu-id="13343-210">Das folgende Beispiel ändert die Eigenschaft **DueDateTime** und verwendet die `Prefer: outlook.timezone` Header die datumsspezifische Eigenschaften in der Antwort in der Eastern Standard Time (EST) Ausdrücken angeben.</span><span class="sxs-lookup"><span data-stu-id="13343-210">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTHgwAAA=')

Prefer: outlook.timezone="Eastern Standard Time"
Content-type: application/json
Content-length: 76

{
  "dueDateTime":  {
      "dateTime": "2016-05-06T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```

### <a name="response"></a><span data-ttu-id="13343-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="13343-211">Response</span></span>

<span data-ttu-id="13343-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13343-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

{
    "id": "AAMkADA1MTHgwAAA=",
    "createdDateTime": "2016-04-22T18:19:18.9526004-04:00",
    "lastModifiedDateTime": "2016-04-22T18:38:20.5541528-04:00",
    "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXg==",
    "categories": [
    ],
    "assignedTo": null,
    "body": {
        "contentType": "text",
        "content": ""
    },
    "completedDateTime": null,
    "dueDateTime": {
        "dateTime": "2016-05-06T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "hasAttachments":false,
    "importance": "normal",
    "isReminderOn": false,
    "owner": "Administrator",
    "parentFolderId": "AQMkADA1MTIBEgAAAA==",
    "recurrence": null,
    "reminderDateTime": null,
    "sensitivity": "normal",
    "startDateTime": {
        "dateTime": "2016-05-03T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "status": "notStarted",
    "subject": "Shop for children's weekend"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
