---
title: Kanalnachrichten auflisten
description: 'Ruft die Liste der Nachrichten (ohne die Antworten) in einem Kanal eines Teams ab. Um die Antworten für eine Nachricht abzurufen, rufen Sie die API zum Auflisten der Nachrichtenantworten oder die API zum Abrufen der Nachrichtenantwort auf. '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: bbd2020e85d011b4e94af1d0e56096d4375b41d3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529173"
---
# <a name="list-channel-messages"></a><span data-ttu-id="b3912-104">Kanalnachrichten auflisten</span><span class="sxs-lookup"><span data-stu-id="b3912-104">List channel messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3912-105">Ruft die Liste der [Nachrichten](../resources/chatmessage.md) (ohne die Antworten) in einem [Kanal](../resources/channel.md) eines [Teams](../resources/team.md) ab.</span><span class="sxs-lookup"><span data-stu-id="b3912-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="b3912-106">Um die Antworten für eine Nachricht abzurufen, rufen Sie die API zum [Auflisten der Nachrichtenantworten](channel-get-messagereply.md) oder die API zum [Abrufen der Nachrichtenantwort](channel-list-messagereplies.md) auf.</span><span class="sxs-lookup"><span data-stu-id="b3912-106">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b3912-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b3912-107">Permissions</span></span>
<span data-ttu-id="b3912-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3912-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3912-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3912-110">Permission type</span></span>|<span data-ttu-id="b3912-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3912-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="b3912-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3912-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3912-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3912-113">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="b3912-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3912-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3912-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3912-115">Not supported</span></span>|
|<span data-ttu-id="b3912-116">Application</span><span class="sxs-lookup"><span data-stu-id="b3912-116">Application</span></span>| <span data-ttu-id="b3912-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3912-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3912-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3912-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3912-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b3912-119">Optional query parameters</span></span>
<span data-ttu-id="b3912-120">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) werden derzeit nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3912-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3912-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3912-121">Request headers</span></span>
| <span data-ttu-id="b3912-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b3912-122">Header</span></span>       | <span data-ttu-id="b3912-123">Wert</span><span class="sxs-lookup"><span data-stu-id="b3912-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b3912-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3912-124">Authorization</span></span>  | <span data-ttu-id="b3912-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b3912-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3912-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3912-127">Request body</span></span>
<span data-ttu-id="b3912-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b3912-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3912-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3912-129">Response</span></span>

<span data-ttu-id="b3912-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [chatmessage](../resources/chatmessage.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3912-130">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/chatmessage.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3912-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3912-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3912-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3912-132">Request</span></span>
<span data-ttu-id="b3912-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b3912-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_messages"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="b3912-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3912-134">Response</span></span>
<span data-ttu-id="b3912-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b3912-135">Here is an example of the response.</span></span> 

><span data-ttu-id="b3912-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b3912-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "content": "Hello World",
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
  "description": "Get channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list-messages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
