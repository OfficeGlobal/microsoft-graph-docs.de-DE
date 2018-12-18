---
title: Ereignisse auflisten
description: Dient zum Abrufen einer Liste von Ereignisobjekten.
author: dkershaw10
ms.openlocfilehash: 12ad3cd2704d31b68aec033381b9c6c5bc23a7fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349161"
---
# <a name="list-events"></a><span data-ttu-id="f54b4-103">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="f54b4-103">List events</span></span>
<span data-ttu-id="f54b4-104">Mit dieser API können Sie eine Liste von Objekten des Typs [event](../resources/event.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="f54b4-104">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f54b4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f54b4-105">Permissions</span></span>
<span data-ttu-id="f54b4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f54b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f54b4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f54b4-108">Permission type</span></span>      | <span data-ttu-id="f54b4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f54b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f54b4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f54b4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f54b4-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f54b4-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f54b4-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f54b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f54b4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f54b4-113">Not supported.</span></span>    |
|<span data-ttu-id="f54b4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f54b4-114">Application</span></span> | <span data-ttu-id="f54b4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f54b4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f54b4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f54b4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f54b4-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f54b4-117">Optional query parameters</span></span>
<span data-ttu-id="f54b4-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f54b4-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f54b4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f54b4-119">Request headers</span></span>
| <span data-ttu-id="f54b4-120">Name</span><span class="sxs-lookup"><span data-stu-id="f54b4-120">Name</span></span>       | <span data-ttu-id="f54b4-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f54b4-121">Type</span></span> | <span data-ttu-id="f54b4-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f54b4-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="f54b4-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f54b4-123">Authorization</span></span>  | <span data-ttu-id="f54b4-124">string</span><span class="sxs-lookup"><span data-stu-id="f54b4-124">string</span></span> | <span data-ttu-id="f54b4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f54b4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f54b4-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f54b4-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="f54b4-128">string</span><span class="sxs-lookup"><span data-stu-id="f54b4-128">string</span></span> | <span data-ttu-id="f54b4-129">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="f54b4-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="f54b4-130">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f54b4-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="f54b4-131">Optional.</span><span class="sxs-lookup"><span data-stu-id="f54b4-131">Optional.</span></span> |
| <span data-ttu-id="f54b4-132">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="f54b4-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="f54b4-133">string</span><span class="sxs-lookup"><span data-stu-id="f54b4-133">string</span></span> | <span data-ttu-id="f54b4-134">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="f54b4-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="f54b4-135">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="f54b4-135">Values can be "text" or "html".</span></span> <span data-ttu-id="f54b4-136">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="f54b4-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="f54b4-137">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f54b4-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="f54b4-138">Optional.</span><span class="sxs-lookup"><span data-stu-id="f54b4-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f54b4-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f54b4-139">Request body</span></span>
<span data-ttu-id="f54b4-140">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f54b4-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f54b4-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="f54b4-141">Response</span></span>
<span data-ttu-id="f54b4-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f54b4-142">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f54b4-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f54b4-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f54b4-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f54b4-144">Request</span></span>
<span data-ttu-id="f54b4-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f54b4-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events
```

#### <a name="response"></a><span data-ttu-id="f54b4-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="f54b4-146">Response</span></span>
<span data-ttu-id="f54b4-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f54b4-147">The following is an example of the response.</span></span>
><span data-ttu-id="f54b4-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f54b4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA==",
      "createdDateTime": "2017-07-31T18:59:01.982289Z",
      "lastModifiedDateTime": "2017-09-06T04:29:38.6647687Z",
      "changeKey": "xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
      "categories": [],
      "originalStartTimeZone": "Eastern Standard Time",
      "originalEndTimeZone": "Eastern Standard Time",
      "iCalUId": "040000008200E00074C5B7101A82E00800000000824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "New Training Plans",
      "bodyPreview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "seriesMaster",
      "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA%3D%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "responseStatus": {
          "response": "organizer",
          "time": "0001-01-01T00:00:00Z"
      },
      "body": {
          "contentType": "html",
          "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Meeting to plan new trainings.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
      },
      "start": {
          "dateTime": "2017-08-14T21:00:00.0000000",
          "timeZone": "UTC"
      },
      "end": {
          "dateTime": "2017-08-14T22:00:00.0000000",
          "timeZone": "UTC"
      },
      "location": {
          "displayName": "HR Taskforce / Facilities"
      },
      "recurrence": {
          "pattern": {
              "type": "weekly",
              "interval": 1,
              "month": 0,
              "dayOfMonth": 0,
              "daysOfWeek": [
                  "monday",
                  "wednesday",
                  "friday"
              ],
              "firstDayOfWeek": "sunday",
              "index": "first"
          },
          "range": {
              "type": "noEnd",
              "startDate": "2017-08-14",
              "endDate": "0001-01-01",
              "recurrenceTimeZone": "Eastern Standard Time",
              "numberOfOccurrences": 0
          }
      },
      "attendees": [
          {
              "type": "required",
              "status": {
                  "response": "accepted",
                  "time": "2017-07-31T18:59:06.4180028Z"
              },
              "emailAddress": {
                  "name": "Joni Sherman",
                  "address": "JoniS@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "HR Taskforce",
                  "address": "HRTaskforce@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Megan Bowen",
                  "address": "MeganB@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Lidia Holloway",
                  "address": "LidiaH@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Emily Braun",
                  "address": "EmilyB@contoso.onmicrosoft.com"
              }
          }
      ],
      "organizer": {
          "emailAddress": {
              "name": "HR Taskforce",
              "address": "HRTaskforce@contoso.onmicrosoft.com"
          }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
