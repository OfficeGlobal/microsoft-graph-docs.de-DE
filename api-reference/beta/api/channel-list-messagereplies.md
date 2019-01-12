---
title: Liste DDE-Kanal an Antworten
description: Listen Sie alle Antworten einer Nachricht in einem Kanal eines Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3648a1eedb53e1838344317c5cd71fe54f8704bf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922242"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="6b678-103">Liste DDE-Kanal an Antworten</span><span class="sxs-lookup"><span data-stu-id="6b678-103">List channel message replies</span></span>

> <span data-ttu-id="6b678-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6b678-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b678-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b678-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b678-106">Listen Sie alle Antworten einer [Nachricht](../resources/chatmessage.md) in einem [Kanal](../resources/channel.md) eines Teams.</span><span class="sxs-lookup"><span data-stu-id="6b678-106">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b678-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6b678-107">Permissions</span></span>
<span data-ttu-id="6b678-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b678-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b678-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6b678-110">Permission Type</span></span>|<span data-ttu-id="6b678-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6b678-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="6b678-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6b678-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b678-113">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b678-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="6b678-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6b678-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b678-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b678-115">Not supported</span></span>|
|<span data-ttu-id="6b678-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6b678-116">Application</span></span>| <span data-ttu-id="6b678-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b678-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b678-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b678-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b678-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6b678-119">Optional query parameters</span></span>
<span data-ttu-id="6b678-120">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) werden derzeit nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b678-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b678-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b678-121">Request headers</span></span>
| <span data-ttu-id="6b678-122">Header</span><span class="sxs-lookup"><span data-stu-id="6b678-122">Header</span></span>       | <span data-ttu-id="6b678-123">Wert</span><span class="sxs-lookup"><span data-stu-id="6b678-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b678-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b678-124">Authorization</span></span>  | <span data-ttu-id="6b678-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6b678-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b678-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6b678-127">Request body</span></span>
<span data-ttu-id="6b678-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6b678-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b678-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b678-129">Response</span></span>
<span data-ttu-id="6b678-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [Chatmessage](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="6b678-130">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b678-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b678-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b678-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b678-132">Request</span></span>
<span data-ttu-id="6b678-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6b678-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message_replies"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
```
##### <a name="response"></a><span data-ttu-id="6b678-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b678-134">Response</span></span>
<span data-ttu-id="6b678-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6b678-135">Here is an example of the response.</span></span> 

><span data-ttu-id="6b678-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6b678-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "value": [
    {
        "id": "id-value",
        "replyToId": "id-value",
        "from" : {
            "user": { 
            "id":  "id-value",
            "displayName": "John Doe"
            }  
        },
        "etag": "id-value",
        "messageType": "message",
        "createdDateTime": "2018-07-09T07:40:20.152Z",
        "lastModifiedDateTime": "2018-07-09T07:40:20.152Z",
        "body": {
            "content": "This is a response to a message.",
            "contentType": "Text"
        },
        "attachments": [
          {
              "id": "5e32f195-168a-474f-a273-123123123",
              "contentType": "reference",
              "contentUrl": "https://test.sharepoint.com/sites/TestSite/Shared%20Documents/General/Test.txt",
              "content": null,
              "name": "Test.txt",
              "thumbnailUrl": null
          }
        ],
        "mentions": [
            {
                "type": "user",
                "id": "id-value ",
                "mentionText": "Test User"
            }
        ],
        "importance": "normal",
        "reactions": [
            {
                "reactionType": "like",
                "user": {
                    "id": "id-value",
                    "displayName": "John Doe"
                },
                "createdDateTime": "2018-07-09T07:40:20.152Z"
            }
        ],
        "locale": "en-us"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
