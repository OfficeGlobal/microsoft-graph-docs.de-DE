---
title: 'conversationThread: reply'
description: 'Beantworten Sie ein Thread in einer gruppenunterhaltung, und fügen Sie eine neue Bereitstellung hinzu. Sie können die übergeordnete Unterhaltung angeben. '
author: dkershaw10
ms.openlocfilehash: 9e439901fd2fa9c37ab30c746628e7fcd771edc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314098"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="eb65e-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="eb65e-104">conversationThread: reply</span></span>

> <span data-ttu-id="eb65e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eb65e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb65e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eb65e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb65e-p103">Dient zum Antworten auf einen Thread in einer Gruppenunterhaltung und zum Hinzufügen eines neuen Beitrags. Sie können die übergeordnete Unterhaltung in der Anforderung angeben, oder Sie können nur den Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="eb65e-p103">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb65e-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eb65e-109">Permissions</span></span>
<span data-ttu-id="eb65e-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb65e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb65e-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb65e-112">Permission type</span></span>      | <span data-ttu-id="eb65e-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb65e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb65e-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb65e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="eb65e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb65e-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb65e-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb65e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb65e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb65e-117">Not supported.</span></span>    |
|<span data-ttu-id="eb65e-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb65e-118">Application</span></span> | <span data-ttu-id="eb65e-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb65e-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb65e-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb65e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="eb65e-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb65e-121">Request headers</span></span>
| <span data-ttu-id="eb65e-122">Header</span><span class="sxs-lookup"><span data-stu-id="eb65e-122">Header</span></span>       | <span data-ttu-id="eb65e-123">Wert</span><span class="sxs-lookup"><span data-stu-id="eb65e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eb65e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb65e-124">Authorization</span></span>  | <span data-ttu-id="eb65e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eb65e-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eb65e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb65e-127">Content-Type</span></span>  | <span data-ttu-id="eb65e-p106">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="eb65e-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eb65e-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb65e-130">Request body</span></span>
<span data-ttu-id="eb65e-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="eb65e-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eb65e-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="eb65e-132">Parameter</span></span>    | <span data-ttu-id="eb65e-133">Typ</span><span class="sxs-lookup"><span data-stu-id="eb65e-133">Type</span></span>   |<span data-ttu-id="eb65e-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb65e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb65e-135">Beitrag</span><span class="sxs-lookup"><span data-stu-id="eb65e-135">post</span></span>|[<span data-ttu-id="eb65e-136">post</span><span class="sxs-lookup"><span data-stu-id="eb65e-136">post</span></span>](../resources/post.md)|<span data-ttu-id="eb65e-137">Der neue Beitrag, mit dem geantwortet wird.</span><span class="sxs-lookup"><span data-stu-id="eb65e-137">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="eb65e-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb65e-138">Response</span></span>

<span data-ttu-id="eb65e-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb65e-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb65e-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb65e-141">Example</span></span>
<span data-ttu-id="eb65e-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="eb65e-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eb65e-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb65e-143">Request</span></span>
<span data-ttu-id="eb65e-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb65e-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/reply
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

##### <a name="response"></a><span data-ttu-id="eb65e-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb65e-145">Response</span></span>
<span data-ttu-id="eb65e-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eb65e-146">Here is an example of the response.</span></span>
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
