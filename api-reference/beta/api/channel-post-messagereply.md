---
title: Antworten auf eine Nachricht in einem Kanal
description: Antworten Sie auf eine Nachricht in einem Kanal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 15e1bfffe7d7634092937a0605debfd5294b142b
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789676"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="a2040-103">Antworten auf eine Nachricht in einem Kanal</span><span class="sxs-lookup"><span data-stu-id="a2040-103">Reply to a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2040-104">Erstellen Sie eine neue Antwort auf eine [Nachricht](../resources/chatmessage.md) in einem angegebenen [Kanal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="a2040-104">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a2040-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a2040-105">Permissions</span></span>
<span data-ttu-id="a2040-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2040-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2040-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2040-108">Permission type</span></span>      | <span data-ttu-id="a2040-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2040-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2040-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2040-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a2040-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2040-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2040-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2040-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2040-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2040-113">Not supported.</span></span>    |
|<span data-ttu-id="a2040-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2040-114">Application</span></span> | <span data-ttu-id="a2040-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2040-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2040-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2040-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="a2040-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2040-117">Request headers</span></span>
| <span data-ttu-id="a2040-118">Name</span><span class="sxs-lookup"><span data-stu-id="a2040-118">Name</span></span>       | <span data-ttu-id="a2040-119">Typ</span><span class="sxs-lookup"><span data-stu-id="a2040-119">Type</span></span> | <span data-ttu-id="a2040-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2040-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2040-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2040-121">Authorization</span></span>  | <span data-ttu-id="a2040-122">string</span><span class="sxs-lookup"><span data-stu-id="a2040-122">string</span></span>  | <span data-ttu-id="a2040-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a2040-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2040-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2040-125">Request body</span></span>
<span data-ttu-id="a2040-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [Message](../resources/chatmessage.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a2040-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="a2040-127">Nur die Body-Eigenschaft ist obligatorisch, andere Eigenschaften sind optional.</span><span class="sxs-lookup"><span data-stu-id="a2040-127">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="a2040-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2040-128">Response</span></span>

<span data-ttu-id="a2040-129">Bei erfolgreicher Ausführung gibt diese Methode `201 Created` den Antwortcode mit der erstellten [Nachricht](../resources/chatmessage.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="a2040-129">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="a2040-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2040-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2040-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2040-131">Request</span></span>
<span data-ttu-id="a2040-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2040-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

##### <a name="response"></a><span data-ttu-id="a2040-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2040-133">Response</span></span>

<span data-ttu-id="a2040-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a2040-134">Here is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
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
  "description": "Create a reply message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-reply_chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
