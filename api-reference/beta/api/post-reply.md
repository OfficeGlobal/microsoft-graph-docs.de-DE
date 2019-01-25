---
title: 'post: reply'
description: 'Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung. Sie können angeben '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: dfdc25b3e99c26d266631a331d7d58c73042e64b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511135"
---
# <a name="post-reply"></a><span data-ttu-id="b4451-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="b4451-104">post: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4451-p102">Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung. Sie können sowohl die übergeordnete Unterhaltung als auch den Thread in der Anforderung angeben, oder Sie können nur den übergeordneten Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="b4451-p102">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4451-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b4451-107">Permissions</span></span>
<span data-ttu-id="b4451-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4451-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4451-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4451-110">Permission type</span></span>      | <span data-ttu-id="b4451-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4451-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4451-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4451-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b4451-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4451-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4451-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4451-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4451-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4451-115">Not supported.</span></span>    |
|<span data-ttu-id="b4451-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4451-116">Application</span></span> | <span data-ttu-id="b4451-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4451-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4451-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4451-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="b4451-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4451-119">Request headers</span></span>
| <span data-ttu-id="b4451-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b4451-120">Header</span></span>       | <span data-ttu-id="b4451-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b4451-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b4451-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4451-122">Authorization</span></span>  | <span data-ttu-id="b4451-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b4451-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4451-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4451-125">Request body</span></span>
<span data-ttu-id="b4451-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b4451-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b4451-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="b4451-127">Parameter</span></span>    | <span data-ttu-id="b4451-128">Typ</span><span class="sxs-lookup"><span data-stu-id="b4451-128">Type</span></span>   |<span data-ttu-id="b4451-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4451-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4451-130">Beitrag</span><span class="sxs-lookup"><span data-stu-id="b4451-130">post</span></span>|[<span data-ttu-id="b4451-131">post</span><span class="sxs-lookup"><span data-stu-id="b4451-131">post</span></span>](../resources/post.md)|<span data-ttu-id="b4451-132">Der neue Beitrag, mit dem geantwortet wird.</span><span class="sxs-lookup"><span data-stu-id="b4451-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="b4451-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4451-133">Response</span></span>

<span data-ttu-id="b4451-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4451-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4451-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4451-136">Example</span></span>
<span data-ttu-id="b4451-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b4451-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b4451-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4451-138">Request</span></span>
<span data-ttu-id="b4451-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4451-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b4451-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4451-140">Response</span></span>
##### <a name="response"></a><span data-ttu-id="b4451-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4451-141">Response</span></span>
<span data-ttu-id="b4451-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b4451-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/post-reply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
