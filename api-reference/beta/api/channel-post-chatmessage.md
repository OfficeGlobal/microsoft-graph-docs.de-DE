---
title: Senden einer Nachricht in einem Kanal
description: Senden Sie eine neue Nachricht im angegebenen Kanal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 960c5d8164f2681b71bb2c3b46383bb210240bb2
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "30799984"
---
# <a name="send-a-message-to-a-channel"></a><span data-ttu-id="8e8a7-103">Senden einer Nachricht an einen Kanal</span><span class="sxs-lookup"><span data-stu-id="8e8a7-103">Send a message to a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e8a7-104">Erstellen Sie eine neue [Nachricht](../resources/chatmessage.md) im angegebenen [Kanal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="8e8a7-104">Create a new [message](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e8a7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8e8a7-105">Permissions</span></span>
<span data-ttu-id="8e8a7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e8a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e8a7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e8a7-108">Permission type</span></span>      | <span data-ttu-id="8e8a7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e8a7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e8a7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e8a7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8e8a7-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e8a7-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8e8a7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e8a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e8a7-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e8a7-113">Not supported.</span></span>    |
|<span data-ttu-id="8e8a7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e8a7-114">Application</span></span> | <span data-ttu-id="8e8a7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e8a7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e8a7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e8a7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="8e8a7-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e8a7-117">Request headers</span></span>
| <span data-ttu-id="8e8a7-118">Name</span><span class="sxs-lookup"><span data-stu-id="8e8a7-118">Name</span></span>       | <span data-ttu-id="8e8a7-119">Typ</span><span class="sxs-lookup"><span data-stu-id="8e8a7-119">Type</span></span> | <span data-ttu-id="8e8a7-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e8a7-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8e8a7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e8a7-121">Authorization</span></span>  | <span data-ttu-id="8e8a7-122">string</span><span class="sxs-lookup"><span data-stu-id="8e8a7-122">string</span></span>  | <span data-ttu-id="8e8a7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e8a7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e8a7-125">Request body</span></span>
<span data-ttu-id="8e8a7-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [Message](../resources/chatmessage.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="8e8a7-127">Nur die Body-Eigenschaft ist obligatorisch, andere Eigenschaften sind optional.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-127">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="8e8a7-128">Hinweis: das Senden von Nachrichten mit Anlagen und Bildern wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-128">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="8e8a7-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e8a7-129">Response</span></span>

<span data-ttu-id="8e8a7-130">Bei erfolgreicher Ausführung gibt diese Methode `201 Created` den Antwortcode mit der erstellten [Nachricht](../resources/chatmessage.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-130">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="8e8a7-131">Beispiele</span><span class="sxs-lookup"><span data-stu-id="8e8a7-131">Examples</span></span> 

### <a name="example-1-hello-world"></a><span data-ttu-id="8e8a7-132">Beispiel 1: Hello World</span><span class="sxs-lookup"><span data-stu-id="8e8a7-132">Example 1: Hello World</span></span>

##### <a name="request"></a><span data-ttu-id="8e8a7-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e8a7-133">Request</span></span>
<span data-ttu-id="8e8a7-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

##### <a name="response"></a><span data-ttu-id="8e8a7-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e8a7-135">Response</span></span>

<span data-ttu-id="8e8a7-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-mentions"></a><span data-ttu-id="8e8a7-137">Beispiel 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="8e8a7-137">Example 2: @mentions</span></span>

##### <a name="request"></a><span data-ttu-id="8e8a7-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e8a7-138">Request</span></span>
<span data-ttu-id="8e8a7-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World <at id=\"0\">Jane Smith</at>"
  },
  "mentions": [
    {
      "id": 0,
      "mentionText": "Jane Smith",
      "mentioned": {
        "user": {
          "displayName": "Jane Smith",
          "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
          "userIdentityType": "aadUser"
        }
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="8e8a7-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e8a7-140">Response</span></span>

<span data-ttu-id="8e8a7-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World <at id=\"0\">Jane Smith</at>"
    },
    "attachments": [],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Jane Smith",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
                    "displayName": "Jane Smith",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Send message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
