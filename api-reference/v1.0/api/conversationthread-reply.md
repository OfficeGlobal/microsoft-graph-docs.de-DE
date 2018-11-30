---
title: 'conversationThread: reply'
description: 'Beantworten Sie ein Thread in einer gruppenunterhaltung, und fügen Sie eine neue Bereitstellung hinzu. Sie können die übergeordnete Unterhaltung angeben. '
ms.openlocfilehash: ca252cb578c0b04cddead455ca046d13180626e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018587"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="654a5-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="654a5-104">conversationThread: reply</span></span>

<span data-ttu-id="654a5-p102">Dient zum Antworten auf einen Thread in einer Gruppenunterhaltung und zum Hinzufügen eines neuen Beitrags. Sie können die übergeordnete Unterhaltung in der Anforderung angeben, oder Sie können nur den Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="654a5-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="654a5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="654a5-107">Permissions</span></span>
<span data-ttu-id="654a5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="654a5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="654a5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="654a5-110">Permission type</span></span>      | <span data-ttu-id="654a5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="654a5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="654a5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="654a5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="654a5-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="654a5-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="654a5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="654a5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="654a5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="654a5-115">Not supported.</span></span>    |
|<span data-ttu-id="654a5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="654a5-116">Application</span></span> | <span data-ttu-id="654a5-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="654a5-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="654a5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="654a5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="654a5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="654a5-119">Request headers</span></span>
| <span data-ttu-id="654a5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="654a5-120">Header</span></span>       | <span data-ttu-id="654a5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="654a5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="654a5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="654a5-122">Authorization</span></span>  | <span data-ttu-id="654a5-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="654a5-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="654a5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="654a5-125">Content-Type</span></span>  | <span data-ttu-id="654a5-p105">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="654a5-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="654a5-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="654a5-128">Request body</span></span>
<span data-ttu-id="654a5-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="654a5-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="654a5-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="654a5-130">Parameter</span></span>    | <span data-ttu-id="654a5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="654a5-131">Type</span></span>   |<span data-ttu-id="654a5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="654a5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="654a5-133">Beitrag</span><span class="sxs-lookup"><span data-stu-id="654a5-133">post</span></span>|[<span data-ttu-id="654a5-134">post</span><span class="sxs-lookup"><span data-stu-id="654a5-134">post</span></span>](../resources/post.md)|<span data-ttu-id="654a5-135">Der neue Beitrag, mit dem geantwortet wird.</span><span class="sxs-lookup"><span data-stu-id="654a5-135">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="654a5-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="654a5-136">Response</span></span>

<span data-ttu-id="654a5-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="654a5-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="654a5-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="654a5-139">Example</span></span>
<span data-ttu-id="654a5-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="654a5-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="654a5-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="654a5-141">Request</span></span>
<span data-ttu-id="654a5-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="654a5-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="654a5-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="654a5-143">Response</span></span>
<span data-ttu-id="654a5-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="654a5-144">Here is an example of the response.</span></span>
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