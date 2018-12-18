---
title: 'conversationThread: reply'
description: 'Beantworten Sie ein Thread in einer gruppenunterhaltung, und fügen Sie eine neue Bereitstellung hinzu. Sie können die übergeordnete Unterhaltung angeben. '
author: dkershaw10
ms.openlocfilehash: c31b6dd08aa888c44a8c12044848e96ffd05de57
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353718"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="c5f08-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="c5f08-104">conversationThread: reply</span></span>

<span data-ttu-id="c5f08-p102">Dient zum Antworten auf einen Thread in einer Gruppenunterhaltung und zum Hinzufügen eines neuen Beitrags. Sie können die übergeordnete Unterhaltung in der Anforderung angeben, oder Sie können nur den Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="c5f08-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5f08-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c5f08-107">Permissions</span></span>
<span data-ttu-id="c5f08-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5f08-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f08-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5f08-110">Permission type</span></span>      | <span data-ttu-id="c5f08-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5f08-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5f08-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5f08-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c5f08-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5f08-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c5f08-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5f08-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5f08-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5f08-115">Not supported.</span></span>    |
|<span data-ttu-id="c5f08-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5f08-116">Application</span></span> | <span data-ttu-id="c5f08-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5f08-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5f08-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5f08-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="c5f08-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5f08-119">Request headers</span></span>
| <span data-ttu-id="c5f08-120">Header</span><span class="sxs-lookup"><span data-stu-id="c5f08-120">Header</span></span>       | <span data-ttu-id="c5f08-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c5f08-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c5f08-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5f08-122">Authorization</span></span>  | <span data-ttu-id="c5f08-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c5f08-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c5f08-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5f08-125">Content-Type</span></span>  | <span data-ttu-id="c5f08-p105">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="c5f08-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5f08-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5f08-128">Request body</span></span>
<span data-ttu-id="c5f08-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c5f08-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5f08-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="c5f08-130">Parameter</span></span>    | <span data-ttu-id="c5f08-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c5f08-131">Type</span></span>   |<span data-ttu-id="c5f08-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5f08-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5f08-133">Beitrag</span><span class="sxs-lookup"><span data-stu-id="c5f08-133">post</span></span>|[<span data-ttu-id="c5f08-134">post</span><span class="sxs-lookup"><span data-stu-id="c5f08-134">post</span></span>](../resources/post.md)|<span data-ttu-id="c5f08-135">Der neue Beitrag, mit dem geantwortet wird.</span><span class="sxs-lookup"><span data-stu-id="c5f08-135">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="c5f08-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5f08-136">Response</span></span>

<span data-ttu-id="c5f08-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5f08-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5f08-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5f08-139">Example</span></span>
<span data-ttu-id="c5f08-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c5f08-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c5f08-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5f08-141">Request</span></span>
<span data-ttu-id="c5f08-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5f08-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="c5f08-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5f08-143">Response</span></span>
<span data-ttu-id="c5f08-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c5f08-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
