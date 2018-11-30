---
title: Nachrichten auflisten
description: 'Mit dieser Methode können Sie die Nachrichten im Postfach des angemeldeten Benutzers abrufen (einschließlich der Nachrichten aus den Ordnern „Gelöschte Elemente“ und „Clutter“). '
ms.openlocfilehash: 6647b1c171bc415844d5154438469122161487eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063897"
---
# <a name="list-messages"></a><span data-ttu-id="f7290-103">Nachrichten auflisten</span><span class="sxs-lookup"><span data-stu-id="f7290-103">List messages</span></span>

> <span data-ttu-id="f7290-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f7290-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7290-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7290-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f7290-106">Mit dieser Methode können Sie die Nachrichten im Postfach des angemeldeten Benutzers abrufen (einschließlich der Nachrichten aus den Ordnern „Gelöschte Elemente“ und „Clutter“).</span><span class="sxs-lookup"><span data-stu-id="f7290-106">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="f7290-107">Sie können insbesondere für die Nachrichten filtern und Abrufen nur diejenigen, die ein [erwähnen](../resources/mention.md) des angemeldeten Benutzers enthalten.</span><span class="sxs-lookup"><span data-stu-id="f7290-107">In particular, you can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span>

<span data-ttu-id="f7290-108">Beachten Sie, dass standardmäßig der `GET /me/messages` Vorgang gibt keine **erwähnt** -Eigenschaft zurück.</span><span class="sxs-lookup"><span data-stu-id="f7290-108">Note that by default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="f7290-109">Verwendung der `$expand` Abfragen Parameter, [Details der einzelnen Erwähnung in einer Nachricht zu erhalten](../api/message-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="f7290-109">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#request-2).</span></span>

<span data-ttu-id="f7290-110">Es gibt zwei Szenarien, in dem eine app Nachrichten in einen anderen Benutzer e-Mail-Ordner abrufen:</span><span class="sxs-lookup"><span data-stu-id="f7290-110">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="f7290-111">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="f7290-111">If the app has application permissions, or,</span></span>
* <span data-ttu-id="f7290-112">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen e-Mail-Ordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="f7290-112">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="f7290-113">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="f7290-113">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="f7290-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f7290-114">Permissions</span></span>
<span data-ttu-id="f7290-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7290-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7290-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7290-117">Permission type</span></span>      | <span data-ttu-id="f7290-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7290-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7290-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7290-119">Delegated (work or school account)</span></span> | <span data-ttu-id="f7290-120">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7290-120">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f7290-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7290-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7290-122">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7290-122">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f7290-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7290-123">Application</span></span> | <span data-ttu-id="f7290-124">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7290-124">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7290-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7290-125">HTTP request</span></span>

<span data-ttu-id="f7290-126">So rufen Sie alle Nachrichten in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="f7290-126">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="f7290-127">So rufen Sie Nachrichten in einem spezifischen Ordner in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="f7290-127">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="f7290-128">So rufen Sie alle Nachrichten in das Postfach des Benutzers, die ein **erwähnen** des Benutzers enthalten:</span><span class="sxs-lookup"><span data-stu-id="f7290-128">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7290-129">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f7290-129">Optional query parameters</span></span>
<span data-ttu-id="f7290-130">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f7290-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f7290-131">Sie können die `$filter` Parameter für die **MentionsPreview** -Eigenschaft auf diese Nachrichten erhalten möchten, in denen die angemeldeten Benutzers erwähnt Abfragen.</span><span class="sxs-lookup"><span data-stu-id="f7290-131">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7290-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f7290-132">Request headers</span></span>
| <span data-ttu-id="f7290-133">Name</span><span class="sxs-lookup"><span data-stu-id="f7290-133">Name</span></span>       | <span data-ttu-id="f7290-134">Typ</span><span class="sxs-lookup"><span data-stu-id="f7290-134">Type</span></span> | <span data-ttu-id="f7290-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7290-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f7290-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7290-136">Authorization</span></span>  | <span data-ttu-id="f7290-137">string</span><span class="sxs-lookup"><span data-stu-id="f7290-137">string</span></span>  | <span data-ttu-id="f7290-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f7290-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7290-140">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="f7290-140">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="f7290-141">string</span><span class="sxs-lookup"><span data-stu-id="f7290-141">string</span></span> | <span data-ttu-id="f7290-142">Das Format, in der die **body**- und **uniqueBody**-Eigenschaften zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f7290-142">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="f7290-143">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="f7290-143">Values can be "text" or "html".</span></span> <span data-ttu-id="f7290-144">Wenn die Kopfzeile nicht angegeben ist, werden die **body**- und **uniqueBody**-Eigenschaften im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7290-144">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="f7290-145">Optional.</span><span class="sxs-lookup"><span data-stu-id="f7290-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7290-146">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f7290-146">Request body</span></span>
<span data-ttu-id="f7290-147">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f7290-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7290-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7290-148">Response</span></span>

<span data-ttu-id="f7290-149">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und Auflistung von [Message](../resources/message.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f7290-149">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="f7290-150">Die Standardseitengröße für diese Anforderung liegt bei 10 Nachrichten.</span><span class="sxs-lookup"><span data-stu-id="f7290-150">The default page size for this request is 10 messages.</span></span> 

## <a name="example"></a><span data-ttu-id="f7290-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7290-151">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="f7290-152">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="f7290-152">Request 1</span></span>
<span data-ttu-id="f7290-153">Im erste Beispiel ruft die Top-10-Nachrichten im Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f7290-153">The first example gets the top 10 messages in the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages
```
##### <a name="response-1"></a><span data-ttu-id="f7290-154">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="f7290-154">Response 1</span></span>
<span data-ttu-id="f7290-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7290-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "2016-10-19T10:37:00Z",
      "sentDateTime": "2016-10-19T10:37:00Z",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```


##### <a name="request-2"></a><span data-ttu-id="f7290-158">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="f7290-158">Request 2</span></span>
<span data-ttu-id="f7290-159">Im nächste Beispiel werden alle Nachrichten im Postfach des angemeldeten Benutzers für Benutzer, in denen den Benutzer erwähnt filtert.</span><span class="sxs-lookup"><span data-stu-id="f7290-159">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="f7290-160">Es verwendet `$select` eine Teilmenge der Eigenschaften jeder Nachricht in der Antwort zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7290-160">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="f7290-161">Das Beispiel umfasst auch die URL-Codierung für die Leerzeichen in der Abfragezeichenfolge-Parameter.</span><span class="sxs-lookup"><span data-stu-id="f7290-161">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
##### <a name="response-2"></a><span data-ttu-id="f7290-162">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="f7290-162">Response 2</span></span>
<span data-ttu-id="f7290-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7290-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 987

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages(subject,sender,receivedDateTime,mentionsPreview)",
  "value":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
      "id":"AQMkADJmMTUAAAgVZAAAA",
      "receivedDateTime":"2016-07-21T07:40:21Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/Users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/Messages('AQMkADJmMTUAAAjwVAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAEGj\"",
      "id":"AQMkADJmMTUAAAjwVAAAA",
      "receivedDateTime":"2016-07-21T07:40:20Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

##### <a name="request-3"></a><span data-ttu-id="f7290-166">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="f7290-166">Request 3</span></span>
<span data-ttu-id="f7290-167">Im dritten Beispiel wird gezeigt, wie mit einem `Prefer: outlook.body-content-type="text"` Kopfzeile, die **Text** und das **UniqueBody** Eigenschaften jeder Nachricht im Textformat abgerufen.</span><span class="sxs-lookup"><span data-stu-id="f7290-167">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
##### <a name="response-3"></a><span data-ttu-id="f7290-168">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="f7290-168">Response 3</span></span>
<span data-ttu-id="f7290-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f7290-169">Here is an example of the response.</span></span> 

<!--
Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.
-->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2704

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)",
    "value":[
        {
            "@odata.type":"#microsoft.graph.eventMessageRequest",
            "@odata.etag":"W/\"CwAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj5\"",
            "id":"AAMkAGIAAAoZCfIAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
            "id":"AAMkAGIAAAoZCfHAAA=",
            "subject":"Welcome to our group!",
            "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
            "body":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAAAAjr\"",
            "id":"AQMkAGIAAAIJTQAAAA==",
            "subject":"Welcome aboard!",
            "bodyPreview":"Welcome to the Support group!",
            "body":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->