---
title: Nachricht erstellen
description: Verwenden Sie diese API zum Erstellen eines Entwurfs einer neuen Nachricht. Entwürfe können in einem beliebigen Ordner erstellt und optional vor dem Senden aktualisiert werden. Verwenden Sie die Verknüpfung „/messages“, um den Entwurf im Ordner „Entwürfe“ zu speichern.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 95fb4c385da7115480a2e1e63135bd875a80b598
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952902"
---
# <a name="create-message"></a><span data-ttu-id="8deba-105">Nachricht erstellen</span><span class="sxs-lookup"><span data-stu-id="8deba-105">Create Message</span></span>

> <span data-ttu-id="8deba-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8deba-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8deba-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8deba-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8deba-p103">Verwenden Sie diese API zum Erstellen eines Entwurfs einer neuen Nachricht. Entwürfe können in einem beliebigen Ordner erstellt und optional vor dem Senden aktualisiert werden. Verwenden Sie die Verknüpfung „/messages“, um den Entwurf im Ordner „Entwürfe“ zu speichern.</span><span class="sxs-lookup"><span data-stu-id="8deba-p103">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="8deba-111">Beim Erstellen der Entwurfsdatenbank in einem Anruf **POST** , können Sie folgende Aktionen ausführen:</span><span class="sxs-lookup"><span data-stu-id="8deba-111">While creating the draft in the same **POST** call, you can:</span></span>

- <span data-ttu-id="8deba-112">Fügen Sie eine [Anlage](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="8deba-112">Include an [attachment](../resources/attachment.md)</span></span> 
- <span data-ttu-id="8deba-113">Rufen Sie einen anderen Benutzer in der neuen Nachricht mithilfe einer [erwähnen](../resources/mention.md)</span><span class="sxs-lookup"><span data-stu-id="8deba-113">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="8deba-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8deba-114">Permissions</span></span>
<span data-ttu-id="8deba-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8deba-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8deba-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8deba-117">Permission type</span></span>      | <span data-ttu-id="8deba-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8deba-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8deba-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8deba-119">Delegated (work or school account)</span></span> | <span data-ttu-id="8deba-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8deba-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8deba-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8deba-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8deba-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8deba-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8deba-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8deba-123">Application</span></span> | <span data-ttu-id="8deba-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8deba-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8deba-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8deba-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="8deba-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8deba-126">Request headers</span></span>
| <span data-ttu-id="8deba-127">Header</span><span class="sxs-lookup"><span data-stu-id="8deba-127">Header</span></span>       | <span data-ttu-id="8deba-128">Wert</span><span class="sxs-lookup"><span data-stu-id="8deba-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8deba-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8deba-129">Authorization</span></span>  | <span data-ttu-id="8deba-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8deba-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8deba-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8deba-132">Content-Type</span></span>  | <span data-ttu-id="8deba-133">application/json</span><span class="sxs-lookup"><span data-stu-id="8deba-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8deba-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8deba-134">Request body</span></span>
<span data-ttu-id="8deba-135">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Message](../resources/message.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8deba-135">In the request body, supply a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="8deba-136">Wenn Sie **erwähnen** aufrufen, um einen anderen Benutzer in der neuen Nachricht verwenden möchten:</span><span class="sxs-lookup"><span data-stu-id="8deba-136">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="8deba-137">Enthalten Sie die erforderlichen **ToRecipients** -Eigenschaft, die **erwähnungen** -Eigenschaft und alle schreibbaren Eigenschaften im Textkörper Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8deba-137">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="8deba-138">Für jede erwähnt werden in der Eigenschaft **erwähnt** müssen Sie die **erwähnten** -Eigenschaft angeben.</span><span class="sxs-lookup"><span data-stu-id="8deba-138">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="8deba-139">Da die **message**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie den `POST`-Vorgang verwenden und während der Erstellung der Nachricht benutzerdefinierte Eigenschaften mit Ihren eigenen Daten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="8deba-139">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="8deba-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="8deba-140">Response</span></span>

<span data-ttu-id="8deba-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und [ein Meldungsobjekt in den Antworttext](../resources/message.md) .</span><span class="sxs-lookup"><span data-stu-id="8deba-141">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8deba-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8deba-142">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="8deba-143">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="8deba-143">Request 1</span></span>
<span data-ttu-id="8deba-144">Hier ist ein Beispiel für die Anforderung zum Erstellen eines Entwurfs oder einer neuen Nachricht ein.</span><span class="sxs-lookup"><span data-stu-id="8deba-144">Here is an example of the request to create a draft of a new message.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject":"Did you see last night's game?",
    "importance":"Low",
    "body":{
        "contentType":"HTML",
        "content":"They were <b>awesome</b>!"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ]
}
```
<span data-ttu-id="8deba-145">Geben Sie im Anforderungstext eine JSON-Darstellung des [message](../resources/message.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8deba-145">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="8deba-146">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="8deba-146">Response 1</span></span>
<span data-ttu-id="8deba-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8deba-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('ad787b4f-1fda-4523-8e48-ffedb7f4635f')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAAmXr9SsE/UR4PcnTZcg7qWAAAFS12t\"",
    "id":"AAMkAGRWAAAFSmKXAAA=",
    "createdDateTime":"2017-12-23T07:29:57Z",
    "lastModifiedDateTime":"2017-12-23T07:29:58Z",
    "changeKey":"CQAAABYAAAAmXr9SsE/UR4PcnTZcg7qWAAAFS12t",
    "categories":[

    ],
    "receivedDateTime":"2017-12-23T07:29:58Z",
    "sentDateTime":"2017-12-23T07:29:58Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR130@MWHPR130.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkAGRWAAAAAAEPAAA=",
    "conversationId":"AAQkAGRVYAsRJrRdc_mWNaxU=",
    "conversationIndex":"AQHTe7/VAniOJVgCxEmtF1z6ZY1rFQ==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkAGRWAAAFSmKXAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "mentionsPreview":null,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"AdeleV@contoso.onmicrosoft.com",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="8deba-150">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="8deba-150">Request 2</span></span>
<span data-ttu-id="8deba-151">Das nächste Beispiel zeigt einen Entwurf e-Mails durch Randi Welch auf Samantha Booth.</span><span class="sxs-lookup"><span data-stu-id="8deba-151">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="8deba-152">Die Nachricht enthält außerdem eine Erwähnung eines anderen Benutzers, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="8deba-152">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="8deba-153">Geben Sie im Anforderungstext eine JSON-Darstellung des [message](../resources/message.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8deba-153">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_with_mentions_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject": "Party planning",
    "toRecipients":[
      {
          "emailAddress":{
              "name":"Samantha Booth",
              "address":"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    "mentions":[
      {    
        "mentioned":{
          "name":"Dana Swope",
          "address":"danas@contoso.onmicrosoft.com"
         }
      }
    ]
}
```


##### <a name="response-2"></a><span data-ttu-id="8deba-154">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="8deba-154">Response 2</span></span>
<span data-ttu-id="8deba-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8deba-p108">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/Messages/$entity",
  "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAW1fsAAAAA==')",
  "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAbYj7\"",
  "id":"AQMkADJmMTUAAAW1fsAAAAA==",
  "body":{
    "contentType":"Text",
    "content":""
  },
  "bodyPreview":"",
  "sender":null,
  "from":null,
  "subject": "Party planning",
  "toRecipients":[
    {
      "emailAddress":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      }
    }
  ],
  "mentionsPreview":{
    "isMentioned":false
  },
  "mentions@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages('AQMkADJmMTUAAAW1fsAAAAA%3D%3D')/mentions",
  "mentions":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAW1fsAAAAA==')/mentions('4577bba4-b063-4cea-9073-6f7ca815fcec')",
      "id":"4577bba4-b063-4cea-9073-6f7ca815fcec",
      "mentioned":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-22T02:22:44Z",
      "serverCreatedDateTime":"2016-07-22T02:22:44.201Z",
      "deepLink":null,
      "application":null
    }
  ]
}

```

##### <a name="request-3"></a><span data-ttu-id="8deba-158">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="8deba-158">Request 3</span></span>
<span data-ttu-id="8deba-159">Im nächste Beispiel fügt eine Reihe von Kunden Internet Nachrichtenkopfzeilen beim Erstellen von e-Mail-Entwurfs.</span><span class="sxs-lookup"><span data-stu-id="8deba-159">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject":"9/8/2018: concert",
    "body":{
        "contentType":"HTML",
        "content":"The group represents Washington."
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "internetMessageHeaders":[
        {
            "name":"x-custom-header-group-name",
            "value":"Washington"
        },
        {
            "name":"x-custom-header-group-id",
            "value":"WA001"
        }
    ]
}
```
<span data-ttu-id="8deba-160">Geben Sie im Anforderungstext eine JSON-Darstellung des [message](../resources/message.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8deba-160">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="8deba-161">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="8deba-161">Response 3</span></span>
<span data-ttu-id="8deba-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8deba-162">Here is an example of the response.</span></span> <span data-ttu-id="8deba-163">Hinweis: Internet Nachrichtenkopfzeilen werden nicht standardmäßig in einer POST-Antwort zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8deba-163">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="8deba-164">Das hier gezeigte Antwortobjekt möglicherweise auch der Kürze halber abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="8deba-164">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="8deba-165">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8deba-165">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_with_headers_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE\"",
    "id":"AAMkADhNmAAA=",
    "createdDateTime":"2018-09-09T02:54:56Z",
    "lastModifiedDateTime":"2018-09-09T02:54:56Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T02:54:56Z",
    "sentDateTime":"2018-09-09T02:54:56Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR220MB1120.namprd22.prod.outlook.com>",
    "subject":"9/8/2018: concert",
    "bodyPreview":"The group represents Washington.",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEPAAA=",
    "conversationId":"AAQkADhNCuP8OKSm-0NE=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhNmAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "mentionsPreview":null,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Washington.\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="8deba-166">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="8deba-166">See also</span></span>

- [<span data-ttu-id="8deba-167">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="8deba-167">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="8deba-168">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="8deba-168">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="8deba-169">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="8deba-169">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
