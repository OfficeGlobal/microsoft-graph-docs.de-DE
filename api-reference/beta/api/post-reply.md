---
title: 'post: reply'
description: 'Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung. Sie können angeben '
author: dkershaw10
ms.openlocfilehash: 33cd99fd24dc5acfca4b96f232f748a0377d1564
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324227"
---
# <a name="post-reply"></a><span data-ttu-id="aece5-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="aece5-104">post: reply</span></span>

> <span data-ttu-id="aece5-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aece5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aece5-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aece5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aece5-p103">Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung. Sie können sowohl die übergeordnete Unterhaltung als auch den Thread in der Anforderung angeben, oder Sie können nur den übergeordneten Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="aece5-p103">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="aece5-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aece5-109">Permissions</span></span>
<span data-ttu-id="aece5-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aece5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aece5-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aece5-112">Permission type</span></span>      | <span data-ttu-id="aece5-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aece5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aece5-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aece5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="aece5-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aece5-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="aece5-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aece5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aece5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aece5-117">Not supported.</span></span>    |
|<span data-ttu-id="aece5-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aece5-118">Application</span></span> | <span data-ttu-id="aece5-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aece5-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aece5-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aece5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="aece5-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aece5-121">Request headers</span></span>
| <span data-ttu-id="aece5-122">Header</span><span class="sxs-lookup"><span data-stu-id="aece5-122">Header</span></span>       | <span data-ttu-id="aece5-123">Wert</span><span class="sxs-lookup"><span data-stu-id="aece5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aece5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aece5-124">Authorization</span></span>  | <span data-ttu-id="aece5-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aece5-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aece5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aece5-127">Request body</span></span>
<span data-ttu-id="aece5-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="aece5-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aece5-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="aece5-129">Parameter</span></span>    | <span data-ttu-id="aece5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="aece5-130">Type</span></span>   |<span data-ttu-id="aece5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aece5-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aece5-132">Beitrag</span><span class="sxs-lookup"><span data-stu-id="aece5-132">post</span></span>|[<span data-ttu-id="aece5-133">post</span><span class="sxs-lookup"><span data-stu-id="aece5-133">post</span></span>](../resources/post.md)|<span data-ttu-id="aece5-134">Der neue Beitrag, mit dem geantwortet wird.</span><span class="sxs-lookup"><span data-stu-id="aece5-134">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="aece5-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="aece5-135">Response</span></span>

<span data-ttu-id="aece5-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aece5-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aece5-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aece5-138">Example</span></span>
<span data-ttu-id="aece5-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="aece5-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aece5-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aece5-140">Request</span></span>
<span data-ttu-id="aece5-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aece5-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "2016-10-19T10:37:00Z",
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
    "createdDateTime": "2016-10-19T10:37:00Z",
    "lastModifiedDateTime": "2016-10-19T10:37:00Z",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "2016-10-19T10:37:00Z",
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

##### <a name="response"></a><span data-ttu-id="aece5-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="aece5-142">Response</span></span>
##### <a name="response"></a><span data-ttu-id="aece5-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="aece5-143">Response</span></span>
<span data-ttu-id="aece5-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aece5-144">Here is an example of the response.</span></span>
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
