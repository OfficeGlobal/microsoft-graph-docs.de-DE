---
title: Unterhaltung erstellen
description: 'Erstellen Sie eine neue Unterhaltung, indem Sie einen Thread und einen Beitrag einschließen. '
author: dkershaw10
ms.openlocfilehash: 48907b41362f56467fbb090e75faa8f3e18720c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340537"
---
# <a name="create-conversation"></a><span data-ttu-id="bc2ad-103">Unterhaltung erstellen</span><span class="sxs-lookup"><span data-stu-id="bc2ad-103">Create conversation</span></span>

> <span data-ttu-id="bc2ad-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc2ad-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc2ad-106">Erstellen Sie eine neue [Unterhaltung](../resources/conversation.md), indem Sie einen Thread und einen Beitrag einschließen.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-106">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="bc2ad-107">Sie können die APIs [conversationThread: reply](conversationthread-reply.md) und [post: reply](post-reply.md) verwenden, um weitere Beiträge in der betreffenden Unterhaltung zu veröffentlichen.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-107">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc2ad-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bc2ad-108">Permissions</span></span>
<span data-ttu-id="bc2ad-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc2ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc2ad-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc2ad-111">Permission type</span></span>      | <span data-ttu-id="bc2ad-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc2ad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc2ad-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc2ad-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bc2ad-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc2ad-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bc2ad-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc2ad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc2ad-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc2ad-116">Not supported.</span></span>    |
|<span data-ttu-id="bc2ad-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc2ad-117">Application</span></span> | <span data-ttu-id="bc2ad-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc2ad-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc2ad-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc2ad-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="bc2ad-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc2ad-120">Request headers</span></span>
| <span data-ttu-id="bc2ad-121">Header</span><span class="sxs-lookup"><span data-stu-id="bc2ad-121">Header</span></span>       | <span data-ttu-id="bc2ad-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bc2ad-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bc2ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc2ad-123">Authorization</span></span>  | <span data-ttu-id="bc2ad-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bc2ad-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc2ad-126">Content-Type</span></span>  | <span data-ttu-id="bc2ad-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bc2ad-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc2ad-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc2ad-128">Request body</span></span>
<span data-ttu-id="bc2ad-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversation](../resources/conversation.md)-Objekts an, das einen [conversationThread](../resources/conversationthread.md) und einen [post](../resources/post.md) enthält.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-129">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="bc2ad-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc2ad-130">Response</span></span>
<span data-ttu-id="bc2ad-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [conversation](../resources/conversation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-131">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span> 

<span data-ttu-id="bc2ad-132">Die Antwort enthält die IDs für die neue Unterhaltung und den Thread, die Sie im Vorgang [Beiträge auflisten](conversationthread-list-posts.md) auch verwenden können, um zu dem neuen Beitrag zu gelangen.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-132">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="bc2ad-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc2ad-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bc2ad-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc2ad-134">Request</span></span>
<span data-ttu-id="bc2ad-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations
Content-type: application/json

{
    "topic":"New head count",
    "threads":[
        {
            "posts":[
                {
                    "body":{
                        "contentType":"html",
                        "content":"The confirmation will come by the end of the week."
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

#### <a name="response"></a><span data-ttu-id="bc2ad-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc2ad-136">Response</span></span>
<span data-ttu-id="bc2ad-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-137">The following is an example of the response.</span></span>
><span data-ttu-id="bc2ad-138">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bc2ad-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
    "id":"AAQkADPxBgqECsrFDTuM=",
    "threads@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADPxBgqECsrFDTuM%3D')/threads",
    "threads":[
        {
            "id":"AAQkADUNO4xAAMbGA93Sw-EGCoQKysUNO4w=="
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