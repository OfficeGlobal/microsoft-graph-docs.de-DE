---
title: eventMessage abrufen
description: Erweitern Sie die Parameter für die Navigation **Event** -Eigenschaft das zugeordnete Ereignis im Kalender des Teilnehmers abgerufen.
localization_priority: Normal
ms.openlocfilehash: ea429ba661d9fd75c45adf50c1cec2bb5a2227cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873815"
---
# <a name="get-eventmessage"></a><span data-ttu-id="53d19-103">eventMessage abrufen</span><span class="sxs-lookup"><span data-stu-id="53d19-103">Get eventMessage</span></span>

<span data-ttu-id="53d19-104">Dient zum Abrufen der Eigenschaften und des [eventMessage](../resources/eventmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="53d19-104">Get the properties and relationships of the [eventMessage](../resources/eventmessage.md) object.</span></span> <span data-ttu-id="53d19-105">Wenden Sie den $expand-Parameter auf die **event**-Navigationseigenschaft an, um das zugewiesene [Ereignis](../resources/event.md) im Kalender des Teilnehmers abzurufen.</span><span class="sxs-lookup"><span data-stu-id="53d19-105">Apply the $expand parameter on the **event** navigation property to get the associated [event](../resources/event.md) in an attendee's calendar.</span></span>

<span data-ttu-id="53d19-106">Zurzeit gibt dieser Vorgang Ereignisnachrichtentext ausschließlich im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="53d19-106">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="53d19-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53d19-107">Permissions</span></span>
<span data-ttu-id="53d19-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53d19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53d19-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53d19-110">Permission type</span></span>      | <span data-ttu-id="53d19-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53d19-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53d19-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53d19-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53d19-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="53d19-113">Mail.Read</span></span>    |
|<span data-ttu-id="53d19-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53d19-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53d19-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="53d19-115">Mail.Read</span></span>    |
|<span data-ttu-id="53d19-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53d19-116">Application</span></span> | <span data-ttu-id="53d19-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="53d19-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="53d19-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53d19-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="53d19-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="53d19-119">Optional query parameters</span></span>
<span data-ttu-id="53d19-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53d19-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="53d19-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53d19-121">Request headers</span></span>
| <span data-ttu-id="53d19-122">Name</span><span class="sxs-lookup"><span data-stu-id="53d19-122">Name</span></span>       | <span data-ttu-id="53d19-123">Typ</span><span class="sxs-lookup"><span data-stu-id="53d19-123">Type</span></span> | <span data-ttu-id="53d19-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53d19-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="53d19-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="53d19-125">Authorization</span></span>  | <span data-ttu-id="53d19-126">string</span><span class="sxs-lookup"><span data-stu-id="53d19-126">string</span></span>  | <span data-ttu-id="53d19-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53d19-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53d19-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53d19-129">Request body</span></span>
<span data-ttu-id="53d19-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="53d19-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53d19-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="53d19-131">Response</span></span>

<span data-ttu-id="53d19-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [eventMessage](../resources/eventmessage.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53d19-132">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53d19-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53d19-133">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="53d19-134">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="53d19-134">Request 1</span></span>
<span data-ttu-id="53d19-135">Das erste Beispiel zeigt, wie Sie die Eigenschaften einer Ereignisnachricht basierend auf der Ereignisnachrichten-ID abrufen.</span><span class="sxs-lookup"><span data-stu-id="53d19-135">The first example shows how to get the properties of an event message based on the event message ID.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAImV_lAAA="],
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADYAAAImV_lAAA=
```
##### <a name="response-1"></a><span data-ttu-id="53d19-136">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="53d19-136">Response 1</span></span>
<span data-ttu-id="53d19-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53d19-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
    "@odata.type":"#microsoft.graph.eventMessage",
    "@odata.etag":"W/\"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVD\"",
    "id":"AAMkADYAAAImV_lAAA=",
    "createdDateTime":"2017-12-27T21:58:36Z",
    "lastModifiedDateTime":"2017-12-27T23:26:38Z",
    "changeKey":"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVD",
    "categories":[

    ],
    "receivedDateTime":"2017-12-27T21:58:36Z",
    "sentDateTime":"2017-12-27T21:58:36Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB2110DCFC@MWHPR1301MB2110.namprd13.prod.outlook.com>",
    "subject":"Debrief from meetup",
    "bodyPreview":"Let's debrief after community meetup.",
    "importance":"normal",
    "parentFolderId":"AQMkADYAAAIBDAAAAA==",
    "conversationId":"AAQkADYCipTiRjXQORU=",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BlAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "meetingMessageType":"meetingRequest",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's debrief after community meetup.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="53d19-140">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="53d19-140">Request 2</span></span>
<span data-ttu-id="53d19-141">Das zweite Beispiel zeigt, wie das mit einer Ereignisnachricht verknüpfte Ereignis abgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="53d19-141">The second example shows how to get the event associated with an event message.</span></span> <span data-ttu-id="53d19-142">Es verwendet die Ereignisnachrichten-ID zum Abrufen der Ereignisnachricht, bietet explizit eine Umwandlung der Ereignisnachricht für den Zugriff auf die **event**-Navigationseigenschaft und wendet einen $expand-Parameter zum Abrufen der Ereigniseigenschaften an.</span><span class="sxs-lookup"><span data-stu-id="53d19-142">It uses the event message ID to get the event message, explicitly provides a cast on the event message to access its **event** navigation property, and apply an $expand parameter to get the properties of the event.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAImV_jAAA="],
  "name": "get_event_based_on_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADYAAAImV_jAAA=?$expand=microsoft.graph.eventMessage/event
```
##### <a name="response-2"></a><span data-ttu-id="53d19-143">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="53d19-143">Response 2</span></span>
<span data-ttu-id="53d19-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53d19-144">Here is an example of the response.</span></span> <span data-ttu-id="53d19-145">Die Eigenschaften des zugeordneten Ereignisses werden in der Antwort zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53d19-145">The properties of the associated event are returned in the response.</span></span> <span data-ttu-id="53d19-146">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="53d19-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="53d19-147">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53d19-147">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_event_based_on_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
   "@odata.type":"#microsoft.graph.eventMessage",
   "@odata.etag":"W/\"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVF\"",
   "id":"AAMkADYAAAImV_jAAA=",
   "createdDateTime":"2017-12-27T21:54:55Z",
   "lastModifiedDateTime":"2017-12-27T23:26:38Z",
   "changeKey":"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVF",
   "categories":[

   ],
   "receivedDateTime":"2017-12-27T21:54:55Z",
   "sentDateTime":"2017-12-27T21:54:54Z",
   "hasAttachments":false,
   "internetMessageId":"<MWHPR1301MB211042CF@MWHPR1301MB2110.namprd13.prod.outlook.com>",
   "subject":"Kick off planning",
   "bodyPreview":"Let's collect opinions from our teams and organize action items.",
   "importance":"normal",
    "parentFolderId":"AQMkADYAS4AAAIBDAAAAA==",
    "conversationId":"AAQkADYRuffB3wDlPn-ReFZarI60=",
   "isDeliveryReceiptRequested":null,
   "isReadReceiptRequested":false,
   "isRead":false,
   "isDraft":false,
   "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BjAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
   "inferenceClassification":"focused",
   "meetingMessageType":"meetingRequest",
   "body":{
      "contentType":"html",
      "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's collect opinions from our teams and organize action items.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
   },
   "sender":{
      "emailAddress":{
         "name":"Administrator",
         "address":"admin@contoso.onmicrosoft.com"
      }
   },
   "from":{
      "emailAddress":{
         "name":"Administrator",
         "address":"admin@contoso.onmicrosoft.com"
      }
   },
   "toRecipients":[
      {
         "emailAddress":{
            "name":"Alex Wilber",
            "address":"AlexW@contoso.onmicrosoft.com"
         }
      }
   ],
   "ccRecipients":[

   ],
   "bccRecipients":[

   ],
   "replyTo":[

   ],
   "event@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages('AAMkADYAAAImV_jAAA%3D')/microsoft.graph.eventMessage/event/$entity",
   "event":{
      "@odata.etag":"W/\"V5Qf0i9DeEOoOqPo0mABLgAACJpBWg==\"",
      "id":"AAMkADYAAAImVu6AAA=",
      "createdDateTime":"2017-12-27T21:54:55.2624551Z",
      "lastModifiedDateTime":"2017-12-27T22:19:16.6667889Z",
      "changeKey":"V5Qf0i9DeEOoOqPo0mABLgAACJpBWg==",
      "categories":[

      ],
      "originalStartTimeZone":"Pacific Standard Time",
      "originalEndTimeZone":"Pacific Standard Time",
      "iCalUId":"040000008200E00074C5B7101A82E00800000000A2A6F3535D7FD3010000000000000000100000003D770E2E8974F44B9471BDB348097FE3",
      "reminderMinutesBeforeStart":15,
      "isReminderOn":true,
      "hasAttachments":false,
      "subject":"Kick off planning",
      "bodyPreview":"Let's collect opinions from our teams and organize action items.",
      "importance":"normal",
      "sensitivity":"normal",
      "isAllDay":false,
      "isCancelled":false,
      "isOrganizer":false,
      "responseRequested":true,
      "seriesMasterId":null,
      "showAs":"tentative",
      "type":"singleInstance",
      "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADYAAAImVu6AAA%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl":null,
      "responseStatus":{
         "response":"tentativelyAccepted",
         "time":"2017-12-27T22:19:12.6197462Z"
      },
      "body":{
         "contentType":"html",
         "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's collect opinions from our teams and organize action items.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
      },
      "start":{
         "dateTime":"2018-02-02T22:00:00.0000000",
         "timeZone":"UTC"
      },
      "end":{
         "dateTime":"2018-02-02T23:00:00.0000000",
         "timeZone":"UTC"
      },
      "location":{
         "displayName":"Mt. Hood"
      },
      "recurrence":null,
      "attendees":[
         {
            "type":"required",
            "status":{
               "response":"none",
               "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
               "name":"Administrator",
               "address":"admin@contoso.onmicrosoft.com"
            }
         },
         {
            "type":"required",
            "status":{
               "response":"tentativelyAccepted",
               "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
               "name":"Alex Wilber",
               "address":"AlexW@contoso.onmicrosoft.com"
            }
         }
      ],
      "organizer":{
         "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
         }
      }
   }
}
``` 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
