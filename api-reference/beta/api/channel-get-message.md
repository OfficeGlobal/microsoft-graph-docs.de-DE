---
title: Kanal-Meldung
description: Rufen Sie eine Nachricht (ohne die Antworten) in einem Kanal eines Teams ab.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 9c8ee3da89beffd78fc906c92a4d2744f168c582
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960882"
---
# <a name="get-channel-message"></a><span data-ttu-id="2e3ac-103">Kanal-Meldung</span><span class="sxs-lookup"><span data-stu-id="2e3ac-103">Get channel message</span></span>

> <span data-ttu-id="2e3ac-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2e3ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e3ac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e3ac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2e3ac-106">Rufen Sie eine [Nachricht](../resources/chatmessage.md) (ohne die Antworten) in einem [Kanal](../resources/channel.md) eines Teams ab.</span><span class="sxs-lookup"><span data-stu-id="2e3ac-106">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e3ac-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2e3ac-107">Permissions</span></span>
<span data-ttu-id="2e3ac-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e3ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e3ac-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e3ac-110">Permission Type</span></span>|<span data-ttu-id="2e3ac-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e3ac-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="2e3ac-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e3ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e3ac-113">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e3ac-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="2e3ac-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e3ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e3ac-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e3ac-115">Not supported</span></span>|
|<span data-ttu-id="2e3ac-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e3ac-116">Application</span></span>| <span data-ttu-id="2e3ac-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e3ac-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e3ac-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e3ac-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e3ac-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2e3ac-119">Optional query parameters</span></span>
<span data-ttu-id="2e3ac-120">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) werden derzeit nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e3ac-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e3ac-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e3ac-121">Request headers</span></span>
| <span data-ttu-id="2e3ac-122">Header</span><span class="sxs-lookup"><span data-stu-id="2e3ac-122">Header</span></span>       | <span data-ttu-id="2e3ac-123">Wert</span><span class="sxs-lookup"><span data-stu-id="2e3ac-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e3ac-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e3ac-124">Authorization</span></span>  | <span data-ttu-id="2e3ac-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2e3ac-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e3ac-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e3ac-127">Request body</span></span>
<span data-ttu-id="2e3ac-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2e3ac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e3ac-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e3ac-129">Response</span></span>

<span data-ttu-id="2e3ac-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [Chatmessage](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="2e3ac-130">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e3ac-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e3ac-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e3ac-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e3ac-132">Request</span></span>
<span data-ttu-id="2e3ac-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e3ac-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="2e3ac-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e3ac-134">Response</span></span>
<span data-ttu-id="2e3ac-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2e3ac-135">Here is an example of the response.</span></span> 

><span data-ttu-id="2e3ac-136">**Hinweis:** Das hier gezeigte Antwortobjekt werden zur besseren Lesbarkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="2e3ac-136">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="2e3ac-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2e3ac-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "replyToId": "id-value",
  "from": {
      "user": { 
        "id": "id-value",
        "displayName": "John Doe"
      }  
  },
  "etag": "id-value",
  "messageType": "message",
  "createdDateTime": "2018-07-09T07:40:20.152Z",
  "lastModifiedDateTime": "2018-07-09T07:40:20.152Z",
  "body": {
      "content": "Hello World",
      "contentType": "text"
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
