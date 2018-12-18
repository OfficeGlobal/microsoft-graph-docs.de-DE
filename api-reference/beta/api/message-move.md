---
title: 'message: move'
description: Verschieben von Nachrichten in einen Ordner. Erstellt eine neue Kopie der Nachricht im Zielordner und die ursprüngliche Nachricht entfernt.
author: angelgolfer-ms
ms.openlocfilehash: 46f62d8793a20db41d19c1677b3d6f48aa7dbd14
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311697"
---
# <a name="message-move"></a><span data-ttu-id="4a32d-104">message: move</span><span class="sxs-lookup"><span data-stu-id="4a32d-104">message: move</span></span>

> <span data-ttu-id="4a32d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4a32d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a32d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4a32d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a32d-107">Verschieben von Nachrichten in einen Ordner.</span><span class="sxs-lookup"><span data-stu-id="4a32d-107">Move a message to a folder.</span></span> <span data-ttu-id="4a32d-108">Erstellt eine neue Kopie der Nachricht im Zielordner und die ursprüngliche Nachricht entfernt.</span><span class="sxs-lookup"><span data-stu-id="4a32d-108">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a32d-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4a32d-109">Permissions</span></span>

<span data-ttu-id="4a32d-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a32d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a32d-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a32d-112">Permission type</span></span> | <span data-ttu-id="4a32d-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a32d-113">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="4a32d-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a32d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4a32d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a32d-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4a32d-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a32d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a32d-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a32d-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4a32d-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a32d-118">Application</span></span> | <span data-ttu-id="4a32d-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a32d-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a32d-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a32d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="4a32d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a32d-121">Request headers</span></span>

| <span data-ttu-id="4a32d-122">Header</span><span class="sxs-lookup"><span data-stu-id="4a32d-122">Header</span></span> | <span data-ttu-id="4a32d-123">Wert</span><span class="sxs-lookup"><span data-stu-id="4a32d-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="4a32d-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4a32d-124">Authorization</span></span> | <span data-ttu-id="4a32d-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="4a32d-125"></span></span> <span data-ttu-id="4a32d-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4a32d-126">Required.</span></span> |
| <span data-ttu-id="4a32d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a32d-127">Content-Type</span></span> | <span data-ttu-id="4a32d-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="4a32d-128"></span></span> <span data-ttu-id="4a32d-129">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4a32d-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a32d-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a32d-130">Request body</span></span>

<span data-ttu-id="4a32d-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="4a32d-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4a32d-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="4a32d-132">Parameter</span></span>   | <span data-ttu-id="4a32d-133">Typ</span><span class="sxs-lookup"><span data-stu-id="4a32d-133">Type</span></span> |<span data-ttu-id="4a32d-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a32d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a32d-135">DestinationId</span><span class="sxs-lookup"><span data-stu-id="4a32d-135">DestinationId</span></span>|<span data-ttu-id="4a32d-136">String</span><span class="sxs-lookup"><span data-stu-id="4a32d-136">String</span></span>|<span data-ttu-id="4a32d-137">Die Ziel-Ordner-ID oder den Ordnernamen einer bekannten.</span><span class="sxs-lookup"><span data-stu-id="4a32d-137">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="4a32d-138">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="4a32d-138">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="4a32d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a32d-139">Response</span></span>

<span data-ttu-id="4a32d-140">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und eine [Nachricht](../resources/message.md) Ressource in den Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4a32d-140">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a32d-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a32d-141">Example</span></span>

<span data-ttu-id="4a32d-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4a32d-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4a32d-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a32d-143">Request</span></span>

<span data-ttu-id="4a32d-144">Die folgende Anforderung verschiebt die angegebene Nachricht in den Ordner Gelöschte Objekte, die anhand des Namens bekannte Ordner identifiziert `deleteditems`.</span><span class="sxs-lookup"><span data-stu-id="4a32d-144">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```

##### <a name="response"></a><span data-ttu-id="4a32d-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a32d-145">Response</span></span>

<span data-ttu-id="4a32d-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4a32d-146">Here is an example of the response.</span></span>

> <span data-ttu-id="4a32d-147">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="4a32d-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4a32d-148">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4a32d-148">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#message",
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
