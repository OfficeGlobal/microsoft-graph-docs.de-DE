---
title: Senden einer Nachricht in einem Kanal
description: Senden Sie eine neue Nachricht im angegebenen Kanal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 42dcf26a5e67f58668f4bd321a68e684feef237f
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458638"
---
# <a name="send-a-message-to-a-channel"></a><span data-ttu-id="5119d-103">Senden einer Nachricht an einen Kanal</span><span class="sxs-lookup"><span data-stu-id="5119d-103">Send a message to a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5119d-104">Erstellen Sie eine neue [Nachricht](../resources/chatmessage.md) im angegebenen [Kanal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="5119d-104">Create a new [message](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5119d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5119d-105">Permissions</span></span>
<span data-ttu-id="5119d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5119d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5119d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5119d-108">Permission type</span></span>      | <span data-ttu-id="5119d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5119d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5119d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5119d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5119d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5119d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5119d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5119d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5119d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5119d-113">Not supported.</span></span>    |
|<span data-ttu-id="5119d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5119d-114">Application</span></span> | <span data-ttu-id="5119d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5119d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5119d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5119d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="5119d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5119d-117">Request headers</span></span>
| <span data-ttu-id="5119d-118">Name</span><span class="sxs-lookup"><span data-stu-id="5119d-118">Name</span></span>       | <span data-ttu-id="5119d-119">Typ</span><span class="sxs-lookup"><span data-stu-id="5119d-119">Type</span></span> | <span data-ttu-id="5119d-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5119d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5119d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5119d-121">Authorization</span></span>  | <span data-ttu-id="5119d-122">string</span><span class="sxs-lookup"><span data-stu-id="5119d-122">string</span></span>  | <span data-ttu-id="5119d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5119d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5119d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5119d-125">Request body</span></span>
<span data-ttu-id="5119d-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [Message](../resources/chatmessage.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5119d-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="5119d-127">Nur die Body-Eigenschaft ist obligatorisch, andere Eigenschaften sind optional.</span><span class="sxs-lookup"><span data-stu-id="5119d-127">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="5119d-128">Hinweis: das Senden von Nachrichten mit Anlagen und Bildern wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5119d-128">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="5119d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5119d-129">Response</span></span>

<span data-ttu-id="5119d-130">Bei erfolgreicher Ausführung gibt diese Methode `201 Created` den Antwortcode mit der erstellten [Nachricht](../resources/chatmessage.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="5119d-130">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="5119d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5119d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5119d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5119d-132">Request</span></span>
<span data-ttu-id="5119d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5119d-133">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5119d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5119d-134">Response</span></span>

<span data-ttu-id="5119d-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5119d-135">Here is an example of the response.</span></span>
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
