---
title: 'event: delta'
description: Abrufen einer Reihe von Ereignissen, die hinzugefügt, gelöscht oder in einem **CalendarView** (eine Reihe von Ereignissen) aktualisiert wurden
ms.openlocfilehash: 180e017e34e7916b0986a7c9647887ede895726e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060979"
---
# <a name="event-delta"></a><span data-ttu-id="99e3a-103">event: delta</span><span class="sxs-lookup"><span data-stu-id="99e3a-103">event: delta</span></span>

> <span data-ttu-id="99e3a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="99e3a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99e3a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99e3a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99e3a-106">Dient zum Abrufen einer Reihe von Ereignissen, die in einer **calendarView** (ein Bereich von Ereignissen) im Hauptkalender des Benutzers hinzugefügt, gelöscht oder aktualisiert wurden.</span><span class="sxs-lookup"><span data-stu-id="99e3a-106">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>

<span data-ttu-id="99e3a-p102">Ein **delta**-Funktionsaufruf für Ereignisse ähnelt einer `GET /calendarview`-Anforderung für einen Datumsbereich im Hauptkalender des Benutzers, mit der Ausnahme, dass durch entsprechende Anwendung von [Statustoken](/graph/delta-query-overview) in einem oder mehreren dieser Aufrufe inkrementelle Änderungen in der betreffenden Kalenderansicht abgefragt werden können. Dies ermöglicht es Ihnen, einen lokalen Speicher der Ereignisse im Hauptkalender eines Benutzers zu pflegen und zu synchronisieren, ohne dass Sie jedes Mal alle Ereignisse des betreffenden Kalenders vom Server abrufen müssen.</span><span class="sxs-lookup"><span data-stu-id="99e3a-p102">A **delta** function call for events is similar to a `GET /calendarview` request for a range of dates in the user's primary calendar, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in that calender view. This allows you to maintain and synchronize a local store of a user's events in the primary calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="99e3a-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="99e3a-109">Permissions</span></span>
<span data-ttu-id="99e3a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99e3a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="99e3a-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99e3a-112">Permission type</span></span>      | <span data-ttu-id="99e3a-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99e3a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99e3a-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99e3a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="99e3a-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99e3a-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="99e3a-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99e3a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99e3a-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99e3a-117">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="99e3a-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="99e3a-118">Application</span></span> | <span data-ttu-id="99e3a-119">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99e3a-119">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="99e3a-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99e3a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/<id>/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}

```

## <a name="query-parameters"></a><span data-ttu-id="99e3a-121">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="99e3a-121">Query parameters</span></span>

<span data-ttu-id="99e3a-p104">Beim Nachverfolgen von Änderungen in Ereignissen wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL. Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben. In nachfolgenden Anforderungen können Sie die `nextLink`- oder `deltaLink`-URL einfach aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="99e3a-p104">Tracking changes in events incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>


| <span data-ttu-id="99e3a-127">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="99e3a-127">Query parameter</span></span>      | <span data-ttu-id="99e3a-128">Typ</span><span class="sxs-lookup"><span data-stu-id="99e3a-128">Type</span></span>   |<span data-ttu-id="99e3a-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99e3a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99e3a-130">startDateTime</span><span class="sxs-lookup"><span data-stu-id="99e3a-130">startDateTime</span></span>|<span data-ttu-id="99e3a-131">String</span><span class="sxs-lookup"><span data-stu-id="99e3a-131">String</span></span>|<span data-ttu-id="99e3a-p105">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="99e3a-p105">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="99e3a-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="99e3a-134">endDateTime</span></span>|<span data-ttu-id="99e3a-135">String</span><span class="sxs-lookup"><span data-stu-id="99e3a-135">String</span></span>|<span data-ttu-id="99e3a-p106">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="99e3a-p106">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|
| <span data-ttu-id="99e3a-138">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="99e3a-138">$deltatoken</span></span> | <span data-ttu-id="99e3a-139">string</span><span class="sxs-lookup"><span data-stu-id="99e3a-139">string</span></span> | <span data-ttu-id="99e3a-p107">Ein [Statustoken](/graph/delta-query-overview), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Kalenderansicht zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Kalenderansicht an.</span><span class="sxs-lookup"><span data-stu-id="99e3a-p107">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="99e3a-142">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="99e3a-142">$skiptoken</span></span> | <span data-ttu-id="99e3a-143">string</span><span class="sxs-lookup"><span data-stu-id="99e3a-143">string</span></span> | <span data-ttu-id="99e3a-144">Ein [Statustoken](/graph/delta-query-overview), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Kalenderansicht weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="99e3a-144">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="99e3a-p108">Wenn Sie eine Delta-Abfrage für eine Kalenderansicht ausführen, gehen Sie davon aus, dass alle Eigenschaften abgerufen werden, die normalerweise von einer `GET /calendarview`-Anforderung abgerufen werden. `$select` wird in diesem Fall nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99e3a-p108">When you do a delta query on a calendar view, expect to get all the properties you'd normally get from a `GET /calendarview` request. `$select` is not supported in this case.</span></span>


## <a name="request-headers"></a><span data-ttu-id="99e3a-147">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99e3a-147">Request headers</span></span>
| <span data-ttu-id="99e3a-148">Name</span><span class="sxs-lookup"><span data-stu-id="99e3a-148">Name</span></span>       | <span data-ttu-id="99e3a-149">Typ</span><span class="sxs-lookup"><span data-stu-id="99e3a-149">Type</span></span> | <span data-ttu-id="99e3a-150">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99e3a-150">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="99e3a-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="99e3a-151">Authorization</span></span>  | <span data-ttu-id="99e3a-152">string</span><span class="sxs-lookup"><span data-stu-id="99e3a-152">string</span></span>  | <span data-ttu-id="99e3a-p109">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99e3a-p109">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99e3a-155">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99e3a-155">Content-Type</span></span>  | <span data-ttu-id="99e3a-156">string</span><span class="sxs-lookup"><span data-stu-id="99e3a-156">string</span></span>  | <span data-ttu-id="99e3a-p110">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="99e3a-p110">application/json. Required.</span></span> |
| <span data-ttu-id="99e3a-159">Prefer</span><span class="sxs-lookup"><span data-stu-id="99e3a-159">Prefer</span></span> | <span data-ttu-id="99e3a-160">string</span><span class="sxs-lookup"><span data-stu-id="99e3a-160">string</span></span>  | <span data-ttu-id="99e3a-p111">odata.maxpagesize={x}. Optional.</span><span class="sxs-lookup"><span data-stu-id="99e3a-p111">odata.maxpagesize={x}. Optional.</span></span> |
| <span data-ttu-id="99e3a-163">Prefer</span><span class="sxs-lookup"><span data-stu-id="99e3a-163">Prefer</span></span> | <span data-ttu-id="99e3a-164">string</span><span class="sxs-lookup"><span data-stu-id="99e3a-164">string</span></span> | <span data-ttu-id="99e3a-p112">{Time zone}. Optional. Falls kein Wert vorhanden, wird UTC angenommen.</span><span class="sxs-lookup"><span data-stu-id="99e3a-p112">{Time zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="99e3a-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="99e3a-167">Response</span></span>

<span data-ttu-id="99e3a-168">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [event](../resources/event.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99e3a-168">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99e3a-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99e3a-169">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99e3a-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99e3a-170">Request</span></span>

<span data-ttu-id="99e3a-171">Das folgende Beispiel zeigt, wie Sie einen einzelnen **delta**-Funktionsaufruf ausführen und die maximale Anzahl von Ereignissen im Antworttext auf 2 beschränken.</span><span class="sxs-lookup"><span data-stu-id="99e3a-171">The following example shows how to make a single **delta** function call, and limit the maximum number of events in the response body to 2.</span></span>

<span data-ttu-id="99e3a-172">Zum Nachverfolgen von Änderungen in einer Kalenderansicht führen Sie einen oder mehrere **delta**-Funktionsaufrufe mit entsprechenden [Statustoken](/graph/delta-query-overview) aus, um den Satz der inkrementellen Änderungen seit der letzten Delta-Abfrage abzurufen.</span><span class="sxs-lookup"><span data-stu-id="99e3a-172">To track changes in a calendar view, you would make one or more **delta** function calls, with appropriate [state tokens](/graph/delta-query-overview), to get the set of incremental changes since the last delta query.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendarview/delta?startdatetime={start_datetime}&enddatetime={end_datetime}

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="99e3a-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="99e3a-173">Response</span></span>
<span data-ttu-id="99e3a-p113">Wenn die Anforderung erfolgreich ist, enthält die Antwort ein Statustoken, entweder ein _skipToken_ (in einem _@odata.nextLink_-Antwortheader) oder ein _deltaToken_ (in einem _@odata.deltaLink_-Antwortheader). Diese geben an, ob Sie mit der Runde fortfahren sollten oder ob alle Änderungen für diese Runde abgerufen wurden.</span><span class="sxs-lookup"><span data-stu-id="99e3a-p113">If the request is successful, the response would include a state token, which is either a _skipToken_ (in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="99e3a-176">Die Antwort unten zeigt ein _skipToken_ in einem _@odata.nextLink_-Antwortheader.</span><span class="sxs-lookup"><span data-stu-id="99e3a-176">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="99e3a-p114">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99e3a-p114">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 359

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/calendarview/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="99e3a-179">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="99e3a-179">See also</span></span>

- [<span data-ttu-id="99e3a-180">Microsoft Graph-Delta-Abfrage</span><span class="sxs-lookup"><span data-stu-id="99e3a-180">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="99e3a-181">Inkrementelle Änderungen an Ereignissen in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="99e3a-181">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->