---
title: 'message: move'
description: Verschieben von Nachrichten in einen Ordner. Erstellt eine neue Kopie der Nachricht im Zielordner und die ursprüngliche Nachricht entfernt.
ms.openlocfilehash: 3266eb93ab5d0fe95a3c1ba0dc8e5004b6302e03
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019948"
---
# <a name="message-move"></a><span data-ttu-id="e6ca7-104">message: move</span><span class="sxs-lookup"><span data-stu-id="e6ca7-104">message: move</span></span>

<span data-ttu-id="e6ca7-105">Verschieben von Nachrichten in einen Ordner.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-105">Move a message to a folder.</span></span> <span data-ttu-id="e6ca7-106">Erstellt eine neue Kopie der Nachricht im Zielordner und die ursprüngliche Nachricht entfernt.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-106">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6ca7-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e6ca7-107">Permissions</span></span>

<span data-ttu-id="e6ca7-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6ca7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6ca7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6ca7-110">Permission type</span></span> | <span data-ttu-id="e6ca7-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6ca7-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="e6ca7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6ca7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e6ca7-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6ca7-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e6ca7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6ca7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6ca7-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6ca7-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e6ca7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e6ca7-116">Application</span></span> | <span data-ttu-id="e6ca7-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6ca7-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6ca7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6ca7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="e6ca7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6ca7-119">Request headers</span></span>

| <span data-ttu-id="e6ca7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e6ca7-120">Header</span></span> | <span data-ttu-id="e6ca7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e6ca7-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="e6ca7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6ca7-122">Authorization</span></span> | <span data-ttu-id="e6ca7-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-123"></span></span> <span data-ttu-id="e6ca7-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-124">Required.</span></span> |
| <span data-ttu-id="e6ca7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6ca7-125">Content-Type</span></span> | <span data-ttu-id="e6ca7-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-126"></span></span> <span data-ttu-id="e6ca7-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6ca7-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6ca7-128">Request body</span></span>

<span data-ttu-id="e6ca7-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6ca7-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="e6ca7-130">Parameter</span></span>   | <span data-ttu-id="e6ca7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e6ca7-131">Type</span></span> |<span data-ttu-id="e6ca7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6ca7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6ca7-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="e6ca7-133">destinationId</span></span>|<span data-ttu-id="e6ca7-134">String</span><span class="sxs-lookup"><span data-stu-id="e6ca7-134">String</span></span>|<span data-ttu-id="e6ca7-135">Die Ziel-Ordner-ID oder den Ordnernamen einer bekannten.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="e6ca7-136">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="e6ca7-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="e6ca7-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6ca7-137">Response</span></span>

<span data-ttu-id="e6ca7-138">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und eine [Nachricht](../resources/message.md) Ressource in den Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6ca7-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6ca7-139">Example</span></span>

<span data-ttu-id="e6ca7-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e6ca7-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6ca7-141">Request</span></span>

<span data-ttu-id="e6ca7-142">Die folgende Anforderung verschiebt die angegebene Nachricht in den Ordner Gelöschte Objekte, die anhand des Namens bekannte Ordner identifiziert `deleteditems`.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-142">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```

##### <a name="response"></a><span data-ttu-id="e6ca7-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6ca7-143">Response</span></span>

<span data-ttu-id="e6ca7-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-144">Here is an example of the response.</span></span>

> <span data-ttu-id="e6ca7-145">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e6ca7-146">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e6ca7-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#message",
    "@odata.type":"#microsoft.graph.message",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "createdDateTime":"2018-08-12T08:43:22Z",
    "lastModifiedDateTime":"2018-08-15T19:47:54Z",
    "changeKey":"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB",
    "categories":[

    ],
    "receivedDateTime":"2018-08-12T08:43:22Z",
    "sentDateTime":"2018-08-12T08:43:20Z",
    "hasAttachments":false,
    "internetMessageId":"<00535324-5988-4b6a-b9af-d44cf2d0b691@MWHPR2201MB1022.namprd22.prod.outlook.com>",
    "subject":"Undeliverable: Meet for lunch?",
    "bodyPreview":"Delivery has failed to these recipients or groups:\r\n\r\nfannyd@contoso.onmicrosoft.com (fannyd@contoso.onmicrosoft.com)\r\nYour message couldn't be delivered. Despite repeated attempts to deliver your message, querying the Domain Name System (DNS) for the rec",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEKAAA=",
    "conversationId":"AAQkADhJzfbkARFhe5kKhjihSA=",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhAAAW%2FVPeAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html></html>"
    },
    "sender":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"fannyd@contoso.onmicrosoft.com",
                "address":"fannyd@contoso.onmicrosoft.com"
            }
        },
        {
            "emailAddress":{
                "name":"danas@contoso.onmicrosoft.com",
                "address":"danas@contoso.onmicrosoft.com"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->