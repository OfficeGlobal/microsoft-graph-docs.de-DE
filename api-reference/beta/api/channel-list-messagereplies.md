---
title: Liste DDE-Kanal an Antworten
description: Listen Sie alle Antworten einer Nachricht in einem Kanal eines Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4ac3b068e93e370ce981d478c87e573f248695c6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512297"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="64637-103">Liste DDE-Kanal an Antworten</span><span class="sxs-lookup"><span data-stu-id="64637-103">List channel message replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64637-104">Listen Sie alle Antworten einer [Nachricht](../resources/chatmessage.md) in einem [Kanal](../resources/channel.md) eines Teams.</span><span class="sxs-lookup"><span data-stu-id="64637-104">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="64637-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="64637-105">Permissions</span></span>
<span data-ttu-id="64637-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64637-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64637-108">Permission Type</span></span>|<span data-ttu-id="64637-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64637-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="64637-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64637-110">Delegated (work or school account)</span></span>|<span data-ttu-id="64637-111">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64637-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="64637-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64637-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64637-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64637-113">Not supported</span></span>|
|<span data-ttu-id="64637-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64637-114">Application</span></span>| <span data-ttu-id="64637-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64637-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64637-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64637-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64637-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="64637-117">Optional query parameters</span></span>
<span data-ttu-id="64637-118">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) werden derzeit nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64637-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64637-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64637-119">Request headers</span></span>
| <span data-ttu-id="64637-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="64637-120">Header</span></span>       | <span data-ttu-id="64637-121">Wert</span><span class="sxs-lookup"><span data-stu-id="64637-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64637-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64637-122">Authorization</span></span>  | <span data-ttu-id="64637-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="64637-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64637-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64637-125">Request body</span></span>
<span data-ttu-id="64637-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="64637-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64637-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="64637-127">Response</span></span>
<span data-ttu-id="64637-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [Chatmessage](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="64637-128">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64637-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64637-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64637-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64637-130">Request</span></span>
<span data-ttu-id="64637-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64637-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message_replies"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
```
##### <a name="response"></a><span data-ttu-id="64637-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="64637-132">Response</span></span>
<span data-ttu-id="64637-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="64637-133">Here is an example of the response.</span></span> 

><span data-ttu-id="64637-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="64637-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list-messagereplies.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
