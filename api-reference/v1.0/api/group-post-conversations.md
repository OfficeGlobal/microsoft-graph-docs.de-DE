---
title: Unterhaltung erstellen
description: 'Erstellen Sie eine neue Unterhaltung, indem Sie einen Thread und einen Beitrag einschließen. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f8f3868f68918f043974c48ac71f8ff95481b040
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981791"
---
# <a name="create-conversation"></a><span data-ttu-id="d4d21-103">Unterhaltung erstellen</span><span class="sxs-lookup"><span data-stu-id="d4d21-103">Create conversation</span></span>
<span data-ttu-id="d4d21-104">Erstellen Sie eine neue [Unterhaltung](../resources/conversation.md), indem Sie einen Thread und einen Beitrag einschließen.</span><span class="sxs-lookup"><span data-stu-id="d4d21-104">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="d4d21-105">Sie können die APIs [conversationThread: reply](conversationthread-reply.md) und [post: reply](post-reply.md) verwenden, um weitere Beiträge in der betreffenden Unterhaltung zu veröffentlichen.</span><span class="sxs-lookup"><span data-stu-id="d4d21-105">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4d21-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d4d21-106">Permissions</span></span>
<span data-ttu-id="d4d21-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4d21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4d21-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4d21-109">Permission type</span></span>      | <span data-ttu-id="d4d21-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4d21-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4d21-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4d21-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d4d21-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4d21-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d4d21-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4d21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4d21-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4d21-114">Not supported.</span></span>    |
|<span data-ttu-id="d4d21-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4d21-115">Application</span></span> | <span data-ttu-id="d4d21-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4d21-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4d21-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4d21-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="d4d21-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4d21-118">Request headers</span></span>
| <span data-ttu-id="d4d21-119">Header</span><span class="sxs-lookup"><span data-stu-id="d4d21-119">Header</span></span>       | <span data-ttu-id="d4d21-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d4d21-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d4d21-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4d21-121">Authorization</span></span>  | <span data-ttu-id="d4d21-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d4d21-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d4d21-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4d21-124">Content-Type</span></span>  | <span data-ttu-id="d4d21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4d21-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4d21-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4d21-126">Request body</span></span>
<span data-ttu-id="d4d21-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversation](../resources/conversation.md)-Objekts an, das einen [conversationThread](../resources/conversationthread.md) und einen [post](../resources/post.md) enthält.</span><span class="sxs-lookup"><span data-stu-id="d4d21-127">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="d4d21-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4d21-128">Response</span></span>
<span data-ttu-id="d4d21-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [conversation](../resources/conversation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4d21-129">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

<span data-ttu-id="d4d21-130">Die Antwort enthält die IDs für die neue Unterhaltung und den Thread, die Sie im Vorgang [Beiträge auflisten](conversationthread-list-posts.md) auch verwenden können, um zu dem neuen Beitrag zu gelangen.</span><span class="sxs-lookup"><span data-stu-id="d4d21-130">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="d4d21-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4d21-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d4d21-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4d21-132">Request</span></span>
<span data-ttu-id="d4d21-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4d21-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["29981b6a-0e57-42dc-94c9-cd24f5306196"],
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations
Content-type: application/json

{
    "topic":"New locations for this quarter",
    "threads":[
        {
            "posts":[
                {
                    "body":{
                        "contentType":"html",
                        "content":"What do we know so far?"
                    },
                    "newParticipants":[
                        {
                            "emailAddress":{
                                "name":"Adele Vance",
                                "address":"AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="d4d21-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4d21-134">Response</span></span>
<span data-ttu-id="d4d21-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d4d21-135">The following is an example of the response.</span></span>
><span data-ttu-id="d4d21-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d4d21-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
    "id":"AAQkADDVKtMlRp4Txc6k=",
    "threads@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADDVKtMlRp4Txc6k%3D')/threads",
    "threads":[
        {
            "id":"AAQkADQDarUNUq0yVGnhPFzqQ=="
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
