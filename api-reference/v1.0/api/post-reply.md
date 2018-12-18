---
title: 'post: reply'
description: 'Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung. Sie können angeben '
author: dkershaw10
ms.openlocfilehash: d20d7411a2456d30fc5c45f93a194db5574f2672
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353788"
---
# <a name="post-reply"></a><span data-ttu-id="f354a-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="f354a-104">post: reply</span></span>

<span data-ttu-id="f354a-p102">Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung. Sie können sowohl die übergeordnete Unterhaltung als auch den Thread in der Anforderung angeben, oder Sie können nur den übergeordneten Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="f354a-p102">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="f354a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f354a-107">Permissions</span></span>
<span data-ttu-id="f354a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f354a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f354a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f354a-110">Permission type</span></span>      | <span data-ttu-id="f354a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f354a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f354a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f354a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f354a-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f354a-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f354a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f354a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f354a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f354a-115">Not supported.</span></span>    |
|<span data-ttu-id="f354a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f354a-116">Application</span></span> | <span data-ttu-id="f354a-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f354a-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f354a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f354a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="f354a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f354a-119">Request headers</span></span>
| <span data-ttu-id="f354a-120">Header</span><span class="sxs-lookup"><span data-stu-id="f354a-120">Header</span></span>       | <span data-ttu-id="f354a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f354a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f354a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f354a-122">Authorization</span></span>  | <span data-ttu-id="f354a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f354a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f354a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f354a-125">Request body</span></span>
<span data-ttu-id="f354a-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="f354a-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f354a-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="f354a-127">Parameter</span></span>    | <span data-ttu-id="f354a-128">Typ</span><span class="sxs-lookup"><span data-stu-id="f354a-128">Type</span></span>   |<span data-ttu-id="f354a-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f354a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f354a-130">Beitrag</span><span class="sxs-lookup"><span data-stu-id="f354a-130">post</span></span>|[<span data-ttu-id="f354a-131">post</span><span class="sxs-lookup"><span data-stu-id="f354a-131">post</span></span>](../resources/post.md)|<span data-ttu-id="f354a-132">Der neue Beitrag, mit dem geantwortet wird.</span><span class="sxs-lookup"><span data-stu-id="f354a-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="f354a-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f354a-133">Response</span></span>

<span data-ttu-id="f354a-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f354a-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f354a-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f354a-136">Example</span></span>
<span data-ttu-id="f354a-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="f354a-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f354a-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f354a-138">Request</span></span>
<span data-ttu-id="f354a-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f354a-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "datetime-value",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "datetime-value",
    "lastModifiedDateTime": "datetime-value",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "datetime-value",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="f354a-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="f354a-140">Response</span></span>
<span data-ttu-id="f354a-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f354a-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
