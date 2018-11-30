---
title: Nachricht erstellen
description: Verwenden Sie diese API zum Erstellen eines Entwurfs einer neuen Nachricht. Entwürfe können in einem beliebigen Ordner erstellt und optional vor dem Senden aktualisiert werden. Verwenden Sie die Verknüpfung „/messages“, um den Entwurf im Ordner „Entwürfe“ zu speichern.
ms.openlocfilehash: 1774e5a06ea6631881d17839de96a82e8a96ca3a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016646"
---
# <a name="create-message"></a><span data-ttu-id="f49e6-105">Nachricht erstellen</span><span class="sxs-lookup"><span data-stu-id="f49e6-105">Create Message</span></span>

<span data-ttu-id="f49e6-p102">Verwenden Sie diese API zum Erstellen eines Entwurfs einer neuen Nachricht. Entwürfe können in einem beliebigen Ordner erstellt und optional vor dem Senden aktualisiert werden. Verwenden Sie die Verknüpfung „/messages“, um den Entwurf im Ordner „Entwürfe“ zu speichern.</span><span class="sxs-lookup"><span data-stu-id="f49e6-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="f49e6-109">Beim Erstellen des Entwurfs im selben **POST**-Aufruf können Sie eine [Anlage](../resources/attachment.md) hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="f49e6-109">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f49e6-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f49e6-110">Permissions</span></span>
<span data-ttu-id="f49e6-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f49e6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f49e6-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f49e6-113">Permission type</span></span>      | <span data-ttu-id="f49e6-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f49e6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f49e6-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f49e6-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f49e6-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f49e6-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f49e6-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f49e6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f49e6-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f49e6-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f49e6-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f49e6-119">Application</span></span> | <span data-ttu-id="f49e6-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f49e6-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f49e6-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f49e6-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="f49e6-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f49e6-122">Request headers</span></span>
| <span data-ttu-id="f49e6-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f49e6-123">Header</span></span>       | <span data-ttu-id="f49e6-124">Wert</span><span class="sxs-lookup"><span data-stu-id="f49e6-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f49e6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f49e6-125">Authorization</span></span>  | <span data-ttu-id="f49e6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f49e6-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f49e6-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f49e6-128">Content-Type</span></span>  | <span data-ttu-id="f49e6-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f49e6-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f49e6-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f49e6-130">Request body</span></span>
<span data-ttu-id="f49e6-131">Geben Sie im Anforderungstext eine JSON-Darstellung des [message](../resources/message.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f49e6-131">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="f49e6-132">Da die **message**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie den `POST`-Vorgang verwenden und während der Erstellung der Nachricht benutzerdefinierte Eigenschaften mit Ihren eigenen Daten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="f49e6-132">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="f49e6-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f49e6-133">Response</span></span>

<span data-ttu-id="f49e6-134">Bei erfolgreicher Ausführung der Methode werden der Antwortcode `201 Created` und das [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f49e6-134">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f49e6-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f49e6-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="f49e6-136">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="f49e6-136">Request 1</span></span>
<span data-ttu-id="f49e6-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f49e6-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
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
<span data-ttu-id="f49e6-138">Geben Sie im Anforderungstext eine JSON-Darstellung des [message](../resources/message.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f49e6-138">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="f49e6-139">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="f49e6-139">Response 1</span></span>
<span data-ttu-id="f49e6-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f49e6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti\"",
    "id":"AAMkADNlNYjSAAA=",
    "createdDateTime":"2017-07-22T01:53:56Z",
    "lastModifiedDateTime":"2017-07-22T01:53:57Z",
    "changeKey":"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti",
    "categories":[

    ],
    "receivedDateTime":"2017-07-22T01:53:57Z",
    "sentDateTime":"2017-07-22T01:53:57Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB@MWHPR1301MB.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkADNlNWAAAAAAEPAAA=",
    "conversationId":"AAQkADNlNFdXGBnqtY=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADNlNYjSAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
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

##### <a name="request-2"></a><span data-ttu-id="f49e6-143">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="f49e6-143">Request 2</span></span>
<span data-ttu-id="f49e6-144">Im nächste Beispiel fügt eine Reihe von Kunden Internet Nachrichtenkopfzeilen beim Erstellen von e-Mail-Entwurfs.</span><span class="sxs-lookup"><span data-stu-id="f49e6-144">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
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
<span data-ttu-id="f49e6-145">Geben Sie im Anforderungstext eine JSON-Darstellung des [message](../resources/message.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f49e6-145">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-2"></a><span data-ttu-id="f49e6-146">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="f49e6-146">Response 2</span></span>
<span data-ttu-id="f49e6-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f49e6-147">Here is an example of the response.</span></span> <span data-ttu-id="f49e6-148">Hinweis: Internet Nachrichtenkopfzeilen werden nicht standardmäßig in einer POST-Antwort zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f49e6-148">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="f49e6-149">Das hier gezeigte Antwortobjekt möglicherweise auch der Kürze halber abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="f49e6-149">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="f49e6-150">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f49e6-150">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
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

## <a name="see-also"></a><span data-ttu-id="f49e6-151">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="f49e6-151">See also</span></span>

- [<span data-ttu-id="f49e6-152">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="f49e6-152">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f49e6-153">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="f49e6-153">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->