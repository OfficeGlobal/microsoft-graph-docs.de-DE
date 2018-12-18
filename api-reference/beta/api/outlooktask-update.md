---
title: Outlooktask aktualisieren
description: Schreibbare Eigenschaften einer Outlook-Aufgabe zu ändern.
author: angelgolfer-ms
ms.openlocfilehash: 0a162c81ef32cb35e930b000678234ede20e4874
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325704"
---
# <a name="update-outlooktask"></a><span data-ttu-id="03fb4-103">Outlooktask aktualisieren</span><span class="sxs-lookup"><span data-stu-id="03fb4-103">Update outlooktask</span></span>

> <span data-ttu-id="03fb4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="03fb4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03fb4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="03fb4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03fb4-106">Schreibbare Eigenschaften einer Outlook-Aufgabe zu ändern.</span><span class="sxs-lookup"><span data-stu-id="03fb4-106">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="03fb4-107">Die **CompletedDateTime** -Eigenschaft kann durch **die Aktivität** oder explizit durch einen PATCH-Vorgang festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="03fb4-107">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="03fb4-108">Wenn Sie PATCH verwenden, um **CompletedDateTime**festgelegt ist, stellen Sie sicher, legen Sie **Status** auf `completed` sowie.</span><span class="sxs-lookup"><span data-stu-id="03fb4-108">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="03fb4-109">Standardmäßig wird dieses Vorgangs (und die POST, GET und [Abschließen von](../api/outlooktask-complete.md) Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="03fb4-109">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="03fb4-110">Sie können mit dem `Prefer: outlook.timezone`-Header alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darstellen.</span><span class="sxs-lookup"><span data-stu-id="03fb4-110">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="03fb4-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="03fb4-111">Permissions</span></span>
<span data-ttu-id="03fb4-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03fb4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03fb4-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="03fb4-114">Permission type</span></span>      | <span data-ttu-id="03fb4-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="03fb4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03fb4-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="03fb4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="03fb4-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03fb4-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="03fb4-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="03fb4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03fb4-119">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03fb4-119">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="03fb4-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="03fb4-120">Application</span></span> | <span data-ttu-id="03fb4-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="03fb4-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03fb4-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="03fb4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="03fb4-123">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="03fb4-123">Optional request headers</span></span>
| <span data-ttu-id="03fb4-124">Name</span><span class="sxs-lookup"><span data-stu-id="03fb4-124">Name</span></span>       | <span data-ttu-id="03fb4-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03fb4-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="03fb4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="03fb4-126">Authorization</span></span>  | <span data-ttu-id="03fb4-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="03fb4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03fb4-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="03fb4-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="03fb4-130">Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="03fb4-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="03fb4-131">Optional.</span><span class="sxs-lookup"><span data-stu-id="03fb4-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03fb4-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="03fb4-132">Request body</span></span>
<span data-ttu-id="03fb4-p107">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="03fb4-p107">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="03fb4-136">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="03fb4-136">Property</span></span>     | <span data-ttu-id="03fb4-137">Typ</span><span class="sxs-lookup"><span data-stu-id="03fb4-137">Type</span></span>   |<span data-ttu-id="03fb4-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03fb4-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03fb4-139">assignedTo</span><span class="sxs-lookup"><span data-stu-id="03fb4-139">assignedTo</span></span>|<span data-ttu-id="03fb4-140">String</span><span class="sxs-lookup"><span data-stu-id="03fb4-140">String</span></span>|<span data-ttu-id="03fb4-141">Der Name der Person, die die Aufgabe zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="03fb4-141">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="03fb4-142">body</span><span class="sxs-lookup"><span data-stu-id="03fb4-142">body</span></span>|[<span data-ttu-id="03fb4-143">itemBody</span><span class="sxs-lookup"><span data-stu-id="03fb4-143">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="03fb4-144">Der Hauptteil der Aufgabe, die in der Regel Informationen zum Vorgang enthält.</span><span class="sxs-lookup"><span data-stu-id="03fb4-144">The task body that typically contains information about the task.</span></span> <span data-ttu-id="03fb4-145">Beachten Sie, dass nur HTML-Typ unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="03fb4-145">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="03fb4-146">categories</span><span class="sxs-lookup"><span data-stu-id="03fb4-146">categories</span></span>|<span data-ttu-id="03fb4-147">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="03fb4-147">String collection</span></span>|<span data-ttu-id="03fb4-148">Die Kategorien, die dem Vorgang zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="03fb4-148">The categories associated with the task.</span></span>|
|<span data-ttu-id="03fb4-149">changeKey</span><span class="sxs-lookup"><span data-stu-id="03fb4-149">changeKey</span></span>|<span data-ttu-id="03fb4-150">String</span><span class="sxs-lookup"><span data-stu-id="03fb4-150">String</span></span>|<span data-ttu-id="03fb4-151">Die Version des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="03fb4-151">The version of the task.</span></span>|
|<span data-ttu-id="03fb4-152">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="03fb4-152">completedDateTime</span></span>|[<span data-ttu-id="03fb4-153">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="03fb4-153">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="03fb4-154">Das Datum in der angegebenen Zeitzone, dass der Vorgang abgeschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="03fb4-154">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="03fb4-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03fb4-155">createdDateTime</span></span>|<span data-ttu-id="03fb4-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03fb4-156">DateTimeOffset</span></span>|<span data-ttu-id="03fb4-157">Datum und Uhrzeit der Erstellung die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="03fb4-157">The date and time when the task was created.</span></span> <span data-ttu-id="03fb4-158">Standardmäßig ist es in UTC.</span><span class="sxs-lookup"><span data-stu-id="03fb4-158">By default, it is in UTC.</span></span> <span data-ttu-id="03fb4-159">Sie können eine benutzerdefinierte Zeitzone in der Kopfzeile der Anforderung bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="03fb4-159">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="03fb4-160">Wert der Eigenschaft verwendet die ISO 8601-Format.</span><span class="sxs-lookup"><span data-stu-id="03fb4-160">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="03fb4-161">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="03fb4-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="03fb4-162">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="03fb4-162">dueDateTime</span></span>|[<span data-ttu-id="03fb4-163">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="03fb4-163">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="03fb4-164">Das Datum in der angegebenen Zeitzone, die die Aufgabe fertig gestellt werden.</span><span class="sxs-lookup"><span data-stu-id="03fb4-164">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="03fb4-165">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="03fb4-165">hasAttachments</span></span>|<span data-ttu-id="03fb4-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="03fb4-166">Boolean</span></span>|<span data-ttu-id="03fb4-167">Legen Sie auf true zurück, wenn der Vorgang Anlagen hat.</span><span class="sxs-lookup"><span data-stu-id="03fb4-167">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="03fb4-168">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="03fb4-168">importance</span></span>|<span data-ttu-id="03fb4-169">string</span><span class="sxs-lookup"><span data-stu-id="03fb4-169">string</span></span>|<span data-ttu-id="03fb4-170">Die Wichtigkeit des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="03fb4-170">The importance of the event.</span></span> <span data-ttu-id="03fb4-171">Mögliche Werte sind: `low`, `normal` und `high`.</span><span class="sxs-lookup"><span data-stu-id="03fb4-171">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="03fb4-172">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="03fb4-172">isReminderOn</span></span>|<span data-ttu-id="03fb4-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="03fb4-173">Boolean</span></span>|<span data-ttu-id="03fb4-174">Legen Sie auf true zurück, wenn eine Warnung festgelegt ist, um die Benutzer über die Aufgabe zu erinnern.</span><span class="sxs-lookup"><span data-stu-id="03fb4-174">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="03fb4-175">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03fb4-175">lastModifiedDateTime</span></span>|<span data-ttu-id="03fb4-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03fb4-176">DateTimeOffset</span></span>|<span data-ttu-id="03fb4-177">Datum und Uhrzeit der letzten die Aufgabe Änderung.</span><span class="sxs-lookup"><span data-stu-id="03fb4-177">The date and time when the task was last modified.</span></span> <span data-ttu-id="03fb4-178">Standardmäßig ist es in UTC.</span><span class="sxs-lookup"><span data-stu-id="03fb4-178">By default, it is in UTC.</span></span> <span data-ttu-id="03fb4-179">Sie können eine benutzerdefinierte Zeitzone in der Kopfzeile der Anforderung bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="03fb4-179">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="03fb4-180">Wert der Eigenschaft um ISO 8601-Format verwendet und ist immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="03fb4-180">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="03fb4-181">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="03fb4-181">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="03fb4-182">owner</span><span class="sxs-lookup"><span data-stu-id="03fb4-182">owner</span></span>|<span data-ttu-id="03fb4-183">String</span><span class="sxs-lookup"><span data-stu-id="03fb4-183">String</span></span>|<span data-ttu-id="03fb4-184">Der Name der Person, die die Aufgabe erstellt.</span><span class="sxs-lookup"><span data-stu-id="03fb4-184">The name of the person who created the task.</span></span>|
|<span data-ttu-id="03fb4-185">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="03fb4-185">parentFolderId</span></span>|<span data-ttu-id="03fb4-186">String</span><span class="sxs-lookup"><span data-stu-id="03fb4-186">String</span></span>|<span data-ttu-id="03fb4-187">Der eindeutige Bezeichner für die Aufgabe übergeordneten Ordner.</span><span class="sxs-lookup"><span data-stu-id="03fb4-187">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="03fb4-188">recurrence</span><span class="sxs-lookup"><span data-stu-id="03fb4-188">recurrence</span></span>|[<span data-ttu-id="03fb4-189">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="03fb4-189">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="03fb4-190">Das Serienmuster für den Vorgang.</span><span class="sxs-lookup"><span data-stu-id="03fb4-190">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="03fb4-191">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="03fb4-191">reminderDateTime</span></span>|[<span data-ttu-id="03fb4-192">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="03fb4-192">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="03fb4-193">Datum und Zeit für eine Erinnerung des Vorgangs erfolgt.</span><span class="sxs-lookup"><span data-stu-id="03fb4-193">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="03fb4-194">sensitivity</span><span class="sxs-lookup"><span data-stu-id="03fb4-194">sensitivity</span></span>|<span data-ttu-id="03fb4-195">string</span><span class="sxs-lookup"><span data-stu-id="03fb4-195">string</span></span>|<span data-ttu-id="03fb4-196">Gibt die Ebene des Datenschutzes für den Vorgang an.</span><span class="sxs-lookup"><span data-stu-id="03fb4-196">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="03fb4-197">Mögliche Werte: sind `normal`, `personal`, `private` und `confidential`.</span><span class="sxs-lookup"><span data-stu-id="03fb4-197">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="03fb4-198">startDateTime</span><span class="sxs-lookup"><span data-stu-id="03fb4-198">startDateTime</span></span>|[<span data-ttu-id="03fb4-199">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="03fb4-199">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="03fb4-200">Das Datum in der angegebenen Zeitzone, wenn der Vorgang zu beginnen.</span><span class="sxs-lookup"><span data-stu-id="03fb4-200">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="03fb4-201">status</span><span class="sxs-lookup"><span data-stu-id="03fb4-201">status</span></span>|<span data-ttu-id="03fb4-202">string</span><span class="sxs-lookup"><span data-stu-id="03fb4-202">string</span></span>|<span data-ttu-id="03fb4-203">Gibt das Bundesland oder den Fortschritt des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="03fb4-203">Indicates the state or progress of the task.</span></span> <span data-ttu-id="03fb4-204">Mögliche Werte sind: `notStarted`, `inProgress`, `completed`, `waitingOnOthers` und `deferred`.</span><span class="sxs-lookup"><span data-stu-id="03fb4-204">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="03fb4-205">Betreff</span><span class="sxs-lookup"><span data-stu-id="03fb4-205">subject</span></span>|<span data-ttu-id="03fb4-206">String</span><span class="sxs-lookup"><span data-stu-id="03fb4-206">String</span></span>|<span data-ttu-id="03fb4-207">Eine kurze Beschreibung oder Titel des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="03fb4-207">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="03fb4-208">Antwort</span><span class="sxs-lookup"><span data-stu-id="03fb4-208">Response</span></span>

<span data-ttu-id="03fb4-209">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [OutlookTask](../resources/outlooktask.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="03fb4-209">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03fb4-210">Beispiel</span><span class="sxs-lookup"><span data-stu-id="03fb4-210">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03fb4-211">Anforderung</span><span class="sxs-lookup"><span data-stu-id="03fb4-211">Request</span></span>
<span data-ttu-id="03fb4-212">Das folgende Beispiel ändert die Eigenschaft **DueDateTime** und verwendet die `Prefer: outlook.timezone` Header die datumsspezifische Eigenschaften in der Antwort in der Eastern Standard Time (EST) Ausdrücken angeben.</span><span class="sxs-lookup"><span data-stu-id="03fb4-212">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
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
##### <a name="response"></a><span data-ttu-id="03fb4-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="03fb4-213">Response</span></span>
<span data-ttu-id="03fb4-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="03fb4-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->